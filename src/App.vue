<template>
  <div id="app" :class="[showAllCornerNames ? 'show-all-corners' : '', lang]">
    <div class="track-map">
      <div class="inner">
        <svg
          viewBox="0 0 660 530"
          class="main-svg"
          width="6600px"
          height="5300px"
        >
          <defs>
            <path
              d="M246.6 482.9c-.8-.8-1.6-1.7-2.4-2.8l-1.7-2.3c-3.7-5.6-2.8-7-6.9-7.3-2-.1-4.3 0-6.9 4.7a23.2 23.2 0 0 1-5 6.4c-4.2 3.8-8.7 7-14.2 7-5.8 0-7.6-3-14.4-5.2a30.4 30.4 0 0 0-15.4-.6c-2 1-1.8 1.2-3.4 1.4-2.1.2-4-1-5.6-2.6-2.4-2.6-3.4-4.4-5.7-7.4-1.7-2.3-4.5-3.6-6-6.2-1-1.8-.6-2.7-3-4.5-1.6-1.2-8.7-1.1-13.4-2.8-3.7-1.2-3.3-6.1-5.8-9.9-2.4-3.7-14.7-11-21.7-16.9-8.4-8.8-8.7-9.6-12-13.4-3.4-3.8-6.4-6.7-9-10.4a15.6 15.6 0 0 1-3.1-10.9c1-9.8 6.7-17.6 6.8-28.7 0-7.7.6-11.2-1.2-23.8-.7-5-2.4-8.5-4.3-13.3a305 305 0 0 0-15-32.4c-2.2-4-5.3-7-9-9.2-4-2.3-8.8-4.3-13.3-6.6a5.6 5.6 0 0 1-3-6c1-4.4 7.3-4.7 14.7-8.2 9-4.2 13-6.7 18.2-11.2 6.3-5.5 12-9.3 18.1-15.3 4.3-4.2 8-6.8 11.5-13.7 1.9-3.8 3.2-7 4.3-11.4 1.5-6.5.1-12.2 1.1-15.7 1.2-4.2 6-5 6.6-8 .6-3-2.8-6.3-1.2-10.6 1-2.6 7.6-6 12.3-10.2 3.9-3.3 3.3-4.2 7-8.1 7.2-7.7 7.7-6.6 15.3-15.2a24 24 0 0 0 6.4-11.5c1.2-5.9-1.5-11.2-3.6-16-.7-1.5-1.9-2.4-3.8-3.2-1.7-.6-4.3.2-6.1-.5-3-1.2-5-2.1-7.8-4.4-3.6-2.8-5.1-5.3-5.3-7.4-.2-2.7 1.4-3.7 3.4-4.6a53 53 0 0 0 15.4-10.2c2.5-2.6 1.2-5.9 2.7-9.4A23 23 0 0 1 166 77c3.3-3.2 8-4.9 13.7-2.3a57.6 57.6 0 0 1 16.4 11c1.5 1.4 1 6 4.2 5.8 4.3-.1 2.1-3 6.6-5.1 7-3.4 16.7-3.8 23.8-2 3.4.8 7.2 2.8 10.6 2.3 4.4-.7 6-4.4 6.4-6.1.9-4-.1-9.7 2-12.5 2.3-2.9 3.4-4.4 17.5-9 13.4-4.3 18.2-1.8 25-4.5 8-3 14.2-13 20.4-12.6 3.2.2 6.3 2 6.9 5.7 1 6.8-.6 13.5-.7 19.7 0 14 4 21.7 6.7 24.8 5.5 6 11.4 9.5 18 12.6 5.1 2.4 9.2 4.7 16.2 4.8 13.2.2 23.3 0 33.4 2.4a53.4 53.4 0 0 1 18.7 6.9c4.2 2.9 6.6 5.6 10.6 8.1 7.6 4.7 13 6.8 19.2 6 5-.8 11.9-5.4 17.1-9.8 4.5-3.7 8.5-9.4 14.2-10.6 8.6-1.9 12.8-.8 18.5-3.1 5-2 7.6-2.1 9-.8 3.5 3.3.9 7-1.6 8.8-5.8 4.4-15.5 12.2-18.3 13-6.8 1.6-5.5 7.3-4 8.8 3.5 3.5 8.8 1 9.5-1.6.5-1.9 2-3 4.8-5.1a48 48 0 0 1 13-6.4c2.8-1 4.6-2 11.9-2.8 5.3-.6 10.7-7.5 15-13.6 5.4-8 .3-9.3 1.5-13.8 1-3.8 2-7.7 7-11 4.1-3 26.3 4.5 28 5.5 3.9 2.4 5.8 7 9.4 8.8 4.3 2 6 2 9.5 3.6a38 38 0 0 1 10.3 15.3c.2 5-8.4 18.5-3.3 23 4.5 4 5.9 2.8 11 5.3 3.4 1.8 3.4 7.5 3.7 11.4.2 3.8 0 8.9-3 10.5-6.2 3.3-14.6-1.7-21.6.2-3.7 1-2.4 5.9-7 11.8-5.5 6.8-8 14.4-8 18.7 0 6.3.6 14.3 0 20-.2 3-2 6.5-4.7 7.8-4.5 2.3-8.8 1.9-12.5 4.6-4 2.8-6.4 6-10.1 10-3.6 4-4.3 6.4-6.5 11.3-2 4.2-3.6 6-5.9 8.7-2 2.4-5.1 3.5-7.7 5.3-2.5 1.6-4.7 4.3-8.9 5.4-11.3 3-21.9 7.8-32.7 8.6-7 .5-9.5-8.4-16.5-8.3-2.9 0-5.7 1.7-8.2 3.4-4.3 3-8.6 5.1-8.3 8.7 1 11.5 22.4 10.7 28 19.6 2 3 4.7 7 4.2 14-.2 3.9-3.3 7-6.2 9.3-6.6 5.4-29.9 18.6-45.1 27.8L351.8 402c-13.8 8.7-35.7 21.7-41.6 26.1-14.2 10.8-26.5 31-29.7 35.7-2 2.9-8.9 7.7-9.6 9.9-1 2.5-.7 7.4-3.2 9.2-3 2.1-4.7 1.3-7.8 1.3-2.7 0-2 .7-4.9 1.3-1.8.4-5 .3-8.3-2.6"
              id="track"
            />
          </defs>

          <g
            class="section"
            :class="showSection ? 'show' : 'hidden'"
            :style="`--st:${sectionStart};--ed:${sectionEnd}`"
          >
            <use href="#track" class="path"></use>
          </g>

          <use href="#track" class="base base2" />

          <g class="extras">
            <path
              v-for="c in bridges"
              :key="c.en"
              class="bridge"
              :d="`M${w * c.stx} ${h * c.sty}L${w * c.edx} ${h * c.edy}`"
            />
            <path
              class="bridge"
              :d="`M${w * 0.367} ${h * 0.919}L${w * 0.379} ${h * 0.903}`"
            />
          </g>

          <use href="#track" class="base" />

          <g
            class="corner"
            :class="showCorner ? 'show' : 'hidden'"
            :style="`--st:${cornerStart};--ed:${cornerEnd}`"
          >
            <use href="#track" class="path"></use>
          </g>

          <use href="#track" class="progress" />
        </svg>

        <!-- <div
          v-for="c in bridges"
          :key="c.en"
          class="corner-name bridge-name"
          :class="[
            c.pt < p || showAllCornerNames ? 'show' : 'hidden',
            c.h,
            c.v,
            c.pt - 0.001 < p && p < c.pt + 0.001 ? 'highlighted' : '',
          ]"
          :style="`--x:${c.x};--y:${c.y}`"
          @click="setP(c.pt)"
        >
          <div>
            <div>
              <template v-if="lang == 'cn'">{{ c.ch }}</template>
              <template v-if="lang == 'en'">{{ c.en }}</template>
            </div>
          </div>
        </div> -->

        <!-- <div
          v-for="c in sections"
          :key="c.en"
          class="corner-name section-name"
          :class="[
            c.st < p || showAllCornerNames ? 'show' : 'hidden',
            c.h,
            c.v,
            c.st < p && p < c.ed ? 'highlighted' : '',
          ]"
          :style="`--x:${c.x};--y:${c.y}`"
          @click="setP((c.st + c.ed) / 2)"
        >
          <div>
            <div>
              <template v-if="lang == 'cn'">{{ c.ch }}</template>
              <template v-if="lang == 'en'">{{ c.en }}</template>
            </div>
          </div>
        </div> -->

        <div
          v-for="c in corners"
          :key="c.en"
          class="corner-name"
          :class="[
            c.st < p || showAllCornerNames ? 'show' : 'hidden',
            c.h,
            c.v,
            c.st < p && p < c.ed ? 'highlighted' : '',
          ]"
          :style="`--x:${c.x};--y:${c.y}`"
          @click="setP((c.st + c.ed) / 2)"
        >
          <div>
            <div>
              <template v-if="lang == 'cn'">{{ c.ch }}</template>
              <template v-if="lang == 'en'">{{ c.en }}</template>
            </div>
          </div>
        </div>

        <div class="mid">
          <div class="msg" v-if="p == 0">
            <div class="inner">
              <p class="title-font msg-title" v-if="lang == 'cn'">
                纽北赛道地图
              </p>
              <p class="title-font msg-title" v-if="lang == 'en'">
                Nürburgring Map
              </p>
              <p v-if="lang == 'cn'">
                <a
                  href="https://zh.wikipedia.org/zh-hans/%E7%BA%BD%E5%8D%9A%E6%A0%BC%E6%9E%97%E8%B5%9B%E9%81%93"
                  target="_blank"
                  >纽博格林赛道</a
                >（德语：Nürburgring）修筑于 1920
                年代，由于跑道非常长、地形复杂充满挑战性，被认为是世界上最严苛的竞速赛道，其中的北环俗称为"纽北"，又叫"绿色地狱"。这里很多弯道都有独特的名字和故事，通过本地图可以方便爱好者学习。
              </p>
              <p v-if="lang == 'en'">
                <a
                  href="https://en.wikipedia.org/wiki/N%C3%BCrburgring"
                  target="_blank"
                  >Nürburgring</a
                >
                is a German race track built in 1920s, and the North
                Loop(Nordschleife) of it is very famous and challenging for
                racers around the world, through this interactive map you can
                learn the names of the corners in Nürburgring
              </p>
              <div class="indicator">
                <div v-if="lang == 'cn'">向下滚动或点击弯道名查看地图</div>
                <div v-if="lang == 'en'">
                  Scroll or click the corner to start
                </div>
                <svg viewBox="0 0 100 100" class="scroll-arrow">
                  <path d="M10 20l40 30l40 -30" />
                  <path d="M10 60l40 30l40 -30" />
                </svg>
              </div>
            </div>
          </div>

          <div class="title-font miles" v-if="p != 0">
            <span v-if="p > 0">{{ (p * 20.832).toFixed(2) }}</span
            ><span v-else>0.00</span> <em>KM</em>
          </div>
        </div>
      </div>
    </div>

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
        <div class="inner" v-if="currentCorner && p > 0">
          <div
            class="primary skew-n title-font"
            v-if="lang == 'cn' && currentCorner.ch"
            :class="currentCorner.ch == currentCorner.nk ? 'qt' : ''"
          >
            {{ currentCorner.ch }}
          </div>
          <div class="primary skew-n" v-if="lang == 'en' && currentCorner.en">
            {{ currentCorner.en }}
          </div>
          <div
            class="nickname qt skew-n title-font"
            v-if="
              lang == 'cn' &&
              currentCorner.nk &&
              currentCorner.ch != currentCorner.nk
            "
          >
            {{ currentCorner.nk }}
          </div>
          <div class="secondary skew-n" v-if="currentCorner.en">
            <span class="extra" v-if="currentCorner.de">
              <svg viewBox="0 0 5 3" class="skew-p">
                <rect
                  id="black_stripe"
                  width="5"
                  height="3"
                  y="0"
                  x="0"
                  fill="#000"
                />
                <rect
                  id="red_stripe"
                  width="5"
                  height="2"
                  y="1"
                  x="0"
                  fill="#6C6C6C"
                />
                <rect
                  id="gold_stripe"
                  width="5"
                  height="1"
                  y="2"
                  x="0"
                  fill="#DADADA"
                />
              </svg>
              {{ currentCorner.de }}
            </span>
            <span class="extra" v-if="lang == 'cn' && currentCorner.en">
              <svg viewBox="0 0 60 30" class="skew-p">
                <clipPath id="s">
                  <path d="M0,0 v30 h60 v-30 z" />
                </clipPath>
                <clipPath id="t">
                  <path
                    d="M30,15 h30 v15 z v15 h-30 z h-30 v-15 z v-15 h30 z"
                  />
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
                  <path
                    d="M30,0 v30 M0,15 h60"
                    stroke="#fff"
                    stroke-width="10"
                  />
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
          <!-- 弯道详细信息 -->
          <div
            class="more skew-n"
            v-if="currentCorner && currentCorner.more && lang == 'cn'"
            v-html="currentCorner.more"
            style="
              margin-top: 1.5em;
              padding: 1.5em;

              border-radius: 12px;
              color: #2c3e50;
              line-height: 1.8;
              font-size: 15px;

              position: relative;
              transition: all 0.3s ease;
            "
          ></div>
        </div>
      </div>

      <!-- 图片展示 -->
      <div
        class="thumbs modern-gallery"
        v-if="currentCorner && currentCorner.imgs"
        style="
          margin-top: 1.5em;
          display: grid;
          grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
          gap: 1em;
          padding: 1em;
          background: rgba(255, 255, 255, 0.05);
          border-radius: 12px;
          backdrop-filter: blur(8px);
        "
      >
        <div
          class="thumb modern-thumb"
          v-for="img in currentCorner.imgs"
          :key="img.src"
          :class="img.url ? 'has-author' : ''"
          style="
            position: relative;
            border-radius: 8px;
            overflow: hidden;
            box-shadow: 0 4px 16px rgba(0, 0, 0, 0.1);
            transition: all 0.3s ease;
            cursor: pointer;
            background: white;
          "
          @mouseover="
            ($event.currentTarget as HTMLElement).style.transform =
              'scale(1.02)'
          "
          @mouseleave="
            ($event.currentTarget as HTMLElement).style.transform = 'scale(1)'
          "
        >
          <img
            class="skew-n modern-img"
            :src="`https://s.anyway.red/nurburgring/${img.src}!/fh/300/quality/68/progressive/true/ignore-error/true`"
            loading="lazy"
            @click="openModal(img)"
            alt="Corner image"
            style="
              width: 100%;
              height: 150px;
              object-fit: cover;
              border-radius: 8px 8px 0 0;
              transition: all 0.3s ease;
            "
          />
          <div
            class="thumb-info"
            style="
              padding: 0.8em;
              background: white;
              border-radius: 0 0 8px 8px;
            "
          >
            <a
              class="thumb-source modern-source"
              v-if="img.url"
              :href="img.url"
              target="_blank"
              :title="`查看照片来源: ${img.author}`"
              style="
                color: #3498db;
                text-decoration: none;
                font-size: 13px;
                font-weight: 500;
                transition: color 0.3s ease;
              "
              @mouseover="
                ($event.target as HTMLElement).style.color = '#2980b9'
              "
              @mouseleave="
                ($event.target as HTMLElement).style.color = '#3498db'
              "
            >
              <span class="skew-n">📸 {{ img.author }}</span>
            </a>
            <div v-else style="color: #7f8c8d; font-size: 13px">
              📸 {{ img.author }}
            </div>
          </div>
        </div>
      </div>
    </div>

    <!-- 快速测试按钮 -->
    <!-- <div style="position: fixed; top: 200px; left: 20px; z-index: 1000">
      <button
        @click="setP(0.01)"
        style="
          margin: 2px;
          padding: 5px;
          background: #007acc;
          color: white;
          border: none;
          border-radius: 3px;
        "
      >
        测试萨宾娜 (p=0.01)
      </button>
      <button
        @click="setP(0.41)"
        style="
          margin: 2px;
          padding: 5px;
          background: #007acc;
          color: white;
          border: none;
          border-radius: 3px;
        "
      >
        测试劳达 (p=0.41)
      </button>
    </div> -->

    <!-- 进度指示器 (暂时隐藏) -->
    <!-- <div class="progress-indicator" v-if="p > 0">进度: {{ (p * 100).toFixed(1) }}%</div> -->

    <!-- 控制按钮 -->
    <div class="controls">
      <button @click="toggleLang" class="control-btn">
        {{ lang === "cn" ? "EN" : "中文" }}
      </button>
      <button @click="toggleAllCornerNames" class="control-btn">
        {{ showAllCornerNames ? "隐藏所有" : "显示所有" }}
      </button>
    </div>

    <!-- 图片模态框 -->
    <div
      class="modal image"
      :class="showModal ? 'show' : ''"
      @click="closeModal"
      v-if="modalImage"
    >
      <div class="inner" @click.stop>
        <div class="modal-content skew-n">
          <img :src="modalImage.src" :alt="modalImage.author" />
          <div class="source-in-modal" v-if="modalImage.url">
            <a :href="modalImage.url" target="_blank">{{
              modalImage.author
            }}</a>
          </div>
        </div>
        <div class="modal-close skew-n" @click="closeModal">
          <svg viewBox="0 0 30 30">
            <circle cx="15" cy="15" r="12" />
            <path d="M10 10L20 20M20 10L10 20" />
          </svg>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup lang="ts">
import { ref, computed, onMounted, onUnmounted } from "vue";
import { useTrackData } from "./composables/useTrackData";

// 响应式数据
const p = ref(0);
const w = ref(660);
const h = ref(530);
const lang = ref("cn");
const showAllCornerNames = ref(false);
const showCorner = ref(false);
const showSection = ref(false);
const cornerStart = ref(0);
const cornerEnd = ref(0);
const sectionStart = ref(0);
const sectionEnd = ref(0);
const scrollDistance = ref(0);
const showModal = ref(false);
const modalImage = ref<{ src: string; url: string; author: string } | null>(
  null
);

// 获取赛道数据
const { bridges, sections, corners } = useTrackData();

// 计算当前弯道
const currentCorner = computed(() => {
  if (p.value === 0) return null;

  // 查找当前位置对应的弯道
  for (const corner of corners) {
    if (corner.st <= p.value && p.value <= corner.ed) {
      return corner;
    }
  }

  // 查找最近经过的弯道
  const passedCorners = corners.filter((corner) => corner.ed < p.value);
  const data = passedCorners[passedCorners.length - 1] || null;

  return data;
});

// 方法
const setP = (value: number) => {
  p.value = value;
  updateCornerSection();

  // 计算对应的滚动位置并滚动到那里
  const targetScrollPercentage = value * 0.98 + 0.01;
  const docHeight = document.documentElement.scrollHeight - window.innerHeight;
  const targetScrollTop = targetScrollPercentage * docHeight;

  // 平滑滚动到目标位置
  window.scrollTo({
    top: targetScrollTop,
    behavior: "smooth",
  });
};

const toggleLang = () => {
  lang.value = lang.value === "cn" ? "en" : "cn";
};

const toggleAllCornerNames = () => {
  showAllCornerNames.value = !showAllCornerNames.value;
};

const openModal = (img: { src: string; url?: string; author?: string }) => {
  modalImage.value = {
    src: `https://s.anyway.red/nurburgring/${img.src}!/fh/300/quality/68/progressive/true/ignore-error/true`,
    url: img.url || "",
    author: img.author || "",
  };
  showModal.value = true;
};

const closeModal = () => {
  showModal.value = false;
  modalImage.value = null;
};

const updateCornerSection = () => {
  const corner = currentCorner.value;
  if (corner) {
    showCorner.value = true;
    cornerStart.value = corner.st;
    cornerEnd.value = corner.ed;
  } else {
    showCorner.value = false;
  }

  // 查找当前位置对应的路段
  const currentSection = sections.find(
    (section) => section.st <= p.value && p.value <= section.ed
  );

  if (currentSection) {
    showSection.value = true;
    sectionStart.value = currentSection.st;
    sectionEnd.value = currentSection.ed;
  } else {
    showSection.value = false;
  }
};

// 节流函数
const throttle = (func: () => void, delay: number) => {
  let timeoutId: ReturnType<typeof setTimeout> | null = null;
  let lastExecTime = 0;
  return function () {
    const currentTime = Date.now();

    if (currentTime - lastExecTime > delay) {
      func();
      lastExecTime = currentTime;
    } else {
      if (timeoutId) clearTimeout(timeoutId);
      timeoutId = setTimeout(
        () => {
          func();
          lastExecTime = Date.now();
        },
        delay - (currentTime - lastExecTime)
      );
    }
  };
};

const updateProgress = () => {
  const scrollTop = window.pageYOffset || document.documentElement.scrollTop;
  const docHeight = document.documentElement.scrollHeight - window.innerHeight;
  const scrollPercentage = scrollTop / docHeight;

  scrollDistance.value = scrollTop;

  // 控制scrolled类 - 与原项目保持一致
  if (scrollTop > 2) {
    document.body.classList.add("scrolled");
  } else {
    document.body.classList.remove("scrolled");
  }

  // 根据滚动位置更新进度 - 让整个滚动距离都用来展示赛道进度
  // 移除死区，让整个滚动范围都响应，但保留一个小的缓冲区
  const newP = Math.max(0, Math.min(1, (scrollPercentage - 0.01) / 0.98));

  // 只在值发生变化时更新
  if (Math.abs(newP - p.value) > 0.001) {
    p.value = newP;

    // 使用requestAnimationFrame优化CSS变量更新
    requestAnimationFrame(() => {
      document.documentElement.style.setProperty("--p", p.value.toString());
    });

    updateCornerSection();
  }
};

// 使用节流优化滚动事件
const handleScroll = throttle(updateProgress, 16); // 约60FPS

const updatePageHeight = () => {
  // 增加页面高度，让用户有更长的滚动距离来体验赛道
  // 相当于20.832公里的赛道需要更多的滚动距离来慢慢体验
  document.body.style.height = "9000vh";
};

// 生命周期
onMounted(() => {
  // 设置页面高度以支持滚动
  updatePageHeight();

  // 初始化CSS变量
  document.documentElement.style.setProperty("--p", "0");

  // 监听滚动事件，使用passive选项优化性能
  window.addEventListener("scroll", handleScroll, { passive: true });

  // 检测用户的语言偏好
  const userLang = navigator.language || "en";
  if (userLang.startsWith("zh")) {
    lang.value = "cn";
  }

  // 初始调用一次滚动处理
  handleScroll();

  // 立即检查是否需要添加scrolled类
  const currentScrollTop =
    window.pageYOffset || document.documentElement.scrollTop;
  if (currentScrollTop > 2) {
    document.body.classList.add("scrolled");
  }
});

onUnmounted(() => {
  window.removeEventListener("scroll", handleScroll);
  // 清理CSS变量
  document.documentElement.style.removeProperty("--p");
  // 重置页面高度
  document.body.style.height = "auto";
  // 清理scrolled类
  document.body.classList.remove("scrolled");
});
</script>

<style>
@import url("./assets/main.css");
.root {
  scroll-behavior: smooth;
}
.controls {
  position: fixed;
  top: 20px;
  right: 20px;
  display: flex;
  gap: 10px;
  z-index: 1000;
}

.control-btn {
  padding: 8px 16px;
  background: rgba(0, 0, 0, 0.7);
  color: white;
  border: none;
  border-radius: 4px;
  cursor: pointer;
  font-size: 14px;
  transition: all 0.2s ease;
}

.control-btn:hover {
  background: rgba(0, 0, 0, 0.9);
  transform: translateY(-2px);
}

/* 隐藏原有的样式元素 */
[v-cloak] {
  display: none;
}

/* 优化滚动体验 */
html {
  scroll-behavior: smooth;
}

/* 性能优化 */
.track-map {
  contain: layout style paint;
  will-change: transform;
}

.corner-name {
  transform: translateZ(0); /* 强制硬件加速 */
  contain: layout style;
}

.progress {
  will-change: stroke-dashoffset;
}

/* 进度指示器 */
.progress-indicator {
  position: fixed;
  top: 10px;
  left: 20px;
  background: rgba(0, 0, 0, 0.7);
  color: white;
  padding: 8px 12px;
  border-radius: 4px;
  font-size: 12px;
  z-index: 1000;
  opacity: 0.8;
}

/* 原项目的简单进入/离开动画 */
.corner .path {
  stroke: #ff4757;
  stroke-width: 8px;
  stroke-linecap: butt;
}

.section .path {
  stroke-width: 10px;
  stroke: var(--text1);
  stroke-linecap: butt;
}
</style>
