<template>
  <div class="desc skew-p">
    <div class="logo">
      <div class="inner skew-n">
        <span class="title-font" v-if="lang == 'cn'"
          >纽<span>博格林</span>北<span>环</span>赛道地图</span
        >
        <span class="title-font" v-if="lang == 'en'">Nürburgring Map</span>
        <img src="/assets/logo.svg" alt="纽北赛道地图" />
      </div>
    </div>

    <div class="corner-info">
      <div class="inner" v-if="currentCorner && p > 0" v-cloak>
        <div
          class="primary skew-n title-font"
          v-if="lang == 'cn' && currentCorner.ch"
          :class="currentCorner.ch == currentCorner.nk ? 'qt' : ''"
          v-cloak
        >
          {{ currentCorner.ch }}
        </div>
        <div
          class="primary skew-n"
          v-if="lang == 'en' && currentCorner.en"
          v-cloak
        >
          {{ currentCorner.en }}
        </div>
        <div
          class="nickname qt skew-n title-font"
          v-if="
            lang == 'cn' &&
            currentCorner.nk &&
            currentCorner.ch != currentCorner.nk
          "
          v-cloak
        >
          {{ currentCorner.nk }}
        </div>
        <div class="secondary skew-n" v-if="currentCorner.en" v-cloak>
          <span class="extra" v-if="currentCorner.de">
            <svg viewBox="0 0 5 3" class="skew-p">
              <rect width="5" height="3" y="0" x="0" fill="#000" />
              <rect width="5" height="2" y="1" x="0" fill="#6C6C6C" />
              <rect width="5" height="1" y="2" x="0" fill="#DADADA" />
            </svg>
            {{ currentCorner.de }}
          </span>
          <span class="extra" v-if="lang == 'cn' && currentCorner.en">
            <svg viewBox="0 0 60 30" class="skew-p">
              <clipPath id="s">
                <path d="M0,0 v30 h60 v-30 z" />
              </clipPath>
              <clipPath id="t">
                <path d="M30,15 h30 v15 z v15 h-30 z h-30 v-15 z v-15 h30 z" />
              </clipPath>
              <g clip-path="url(#s)">
                <path d="M0,0 v30 h60 v-30 z" fill="#292929" />
                <path
                  d="M0,0 L60,30 M60,0 L0,30"
                  stroke="#fff"
                  stroke-width="6"
                />
                <path
                  d="M0,0 L60,30 M60,0 L0,30"
                  clip-path="url(#t)"
                  stroke="#646464"
                  stroke-width="4"
                />
                <path d="M30,0 v30 M0,15 h60" stroke="#fff" stroke-width="10" />
                <path
                  d="M30,0 v30 M0,15 h60"
                  stroke="#646464"
                  stroke-width="6"
                />
              </g>
            </svg>
            {{ currentCorner.en }}
          </span>
        </div>
        <div
          class="more skew-n"
          v-if="lang == 'cn' && currentCorner.more"
          v-html="currentCorner.more"
        ></div>
      </div>

      <div class="inner desc-msg" v-if="p == 1" v-cloak>
        <div class="ending skew-n" v-if="p > 0.999">
          The End
          <div class="btn skew-p" @click="$emit('set-p', 0.001)">
            <div class="skew-n title-font" v-if="lang == 'cn'">回到起点</div>
            <div class="skew-n" v-if="lang == 'en'">Start Over</div>
          </div>
        </div>
      </div>

      <div class="thumbs" v-if="currentCorner && currentCorner.imgs" v-cloak>
        <div
          class="thumb"
          v-for="img in currentCorner.imgs"
          :key="img.src"
          :class="img.url ? 'has-author' : ''"
        >
          <img
            class="skew-n"
            :src="`https://s.anyway.red/nurburgring/${img.src}!/fh/300/quality/68/progressive/true/ignore-error/true`"
            loading="lazy"
            @click="$emit('open-modal', 'image', img)"
          />
          <a
            class="thumb-source"
            v-if="img.url"
            :href="img.url"
            target="_blank"
            title="查看照片来源"
            ><span class="skew-n">{{ img.author }}</span></a
          >
        </div>
      </div>
    </div>

    <div class="controls">
      <div class="inner skew-n">
        <div @click="$emit('open-modal', 'text')" role="button" class="link">
          <template v-if="lang == 'cn'">关于本站</template>
          <template v-if="lang == 'en'">About</template>
        </div>

        <div
          class="toggle-group"
          :class="showAllCornerNames ? 'on' : 'off'"
          @click="$emit('toggle-all-corners')"
        >
          <span v-if="lang == 'cn'">所有弯道</span>
          <span v-if="lang == 'en'">All Corners</span>
          <div class="toggle"></div>
        </div>

        <div
          class="toggle-group"
          :class="darkMode ? 'on' : 'off'"
          @click="$emit('toggle-dark-mode')"
        >
          <span v-if="lang == 'cn'">深色模式</span>
          <span v-if="lang == 'en'">Dark Mode</span>
          <div class="toggle"></div>
        </div>

        <div
          class="toggle-group"
          :class="lang == 'cn' ? 'on' : 'off'"
          @click="$emit('toggle-lang')"
        >
          <span v-if="lang == 'cn'">中文</span>
          <span v-if="lang == 'en'">Chinese</span>
          <div class="toggle"></div>
        </div>
      </div>
    </div>

    <div class="all-names title-font">
      <template v-for="c in corners" :key="c.ch">
        {{ c.ch }} <template v-if="c.nk && c.ch != c.nk">{{ c.nk }} </template>
      </template>
    </div>
  </div>
</template>

<script setup>
import { cornerData } from "../data/cornerData.js";

// Props
defineProps({
  lang: String,
  currentCorner: Object,
  p: Number,
  showAllCornerNames: Boolean,
  darkMode: Boolean,
});

// Emits
defineEmits([
  "toggle-all-corners",
  "toggle-dark-mode",
  "toggle-lang",
  "open-modal",
  "set-p",
]);

// Data
const corners = cornerData;
</script>
