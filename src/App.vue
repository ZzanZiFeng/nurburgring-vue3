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
              :key="c.ch"
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

        <!-- Corner Names -->
        <div
          v-for="c in corners"
          :key="c.ch"
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

        <!-- Mid Content -->
        <div class="mid" v-cloak>
          <div class="msg" v-if="p == 0">
            <div class="inner" v-cloak>
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
                >
                （德语：Nürburgring）修筑于 1920
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

    <!-- Description Panel -->
    <DescriptionPanel
      :lang="lang"
      :current-corner="currentCorner"
      :p="p"
      :show-all-corner-names="showAllCornerNames"
      :dark-mode="darkMode"
      @toggle-all-corners="showAllCornerNames = !showAllCornerNames"
      @toggle-dark-mode="toggleDarkMode"
      @toggle-lang="toggleLang"
      @open-modal="openModal"
      @set-p="setP"
    />

    <!-- Modal -->
    <AppModal
      :show="showModal"
      :type="modalType"
      :content="modalContent"
      @close="showModal = false"
    />
  </div>
</template>

<script setup>
import { ref, onMounted, onUnmounted } from "vue";
import DescriptionPanel from "./components/DescriptionPanel.vue";
import AppModal from "./components/AppModal.vue";
import { cornerData, bridgeData, sectionData } from "./data/cornerData.js";

// Reactive state
const p = ref(0);
const w = ref(660);
const h = ref(530);
const lang = ref(detectLanguage());
const showModal = ref(false);
const showAllCornerNames = ref(false);
const darkMode = ref(
  window.matchMedia && window.matchMedia("(prefers-color-scheme: dark)").matches
);
const showCorner = ref(false);
const showSection = ref(false);
const currentCorner = ref(null);
const cornerStart = ref(0);
const cornerEnd = ref(0);
const sectionStart = ref(0);
const sectionEnd = ref(0);
const modalContent = ref("");
const modalType = ref("text");

// Data
const corners = cornerData;
const bridges = bridgeData;
const sections = sectionData;

// Methods
function detectLanguage() {
  const acceptLanguage = navigator.language || navigator.userLanguage;
  if (acceptLanguage.includes("zh")) {
    return "cn";
  }
  return "en";
}

function toggleLang() {
  lang.value = lang.value === "en" ? "cn" : "en";
}

function toggleDarkMode() {
  darkMode.value = !darkMode.value;
  const root = document.querySelector(":root");
  if (darkMode.value) {
    root.classList.add("dark");
  } else {
    root.classList.remove("dark");
  }
}

function setP(percentage) {
  p.value = percentage;
  const body = document.querySelector("body");
  window.scrollTo(0, (body.scrollHeight - window.innerHeight) * percentage);
  updateScrollDistance();
}

function openModal(type, img = null) {
  modalType.value = type;
  if (type === "text") {
    modalContent.value =
      "网页设计 & 开发：<a href='https://jjying.com/' target='_blank'>JJ Ying</a><br/><br/><strong>参考信息:</strong><br/>· <a target='_blank' href='https://oversteer48.com/nurburgring-corner-names/'>Corner Names, Numbers and circuit map</a><br/>· <a target='_blank' href='https://nring.info/nurburgring-nordschleife-corners/'>NRing.info</a><br/>· <a target='_blank' href='https://www.youtube.com/watch?v=-lCR1_cDqTg'>Nürburgring Corner Names Explained</a><br/>· 键盘车神教教主视频：<a target='_blank' href='https://www.bilibili.com/video/BV1NntCe4ETM/'>纽北每一个弯的名字？</a><br/><br/><strong>页面源码:</strong><br/>· <a target='_blank' href='https://github.com/JJYing/Nurburgring-Map'>@GitHub</a>";
  }
  if (type === "image") {
    modalContent.value = `<img src='https://s.anyway.red/nurburgring/${img.src}!/quality/80/progressive/true/ignore-error/true'/>`;
    if (img.url) {
      modalContent.value += `<div class='source-in-modal'>@<a href='${img.url}' target='_blank'>${img.author}</a></div>`;
    }
  }
  showModal.value = true;
}

function updateScrollDistance() {
  showCorner.value = false;
  showSection.value = false;
  currentCorner.value = null;

  const body = document.querySelector("body");
  let progress = window.scrollY / (body.scrollHeight - window.innerHeight);
  if (progress > 1) {
    progress = 1;
  }

  body.style.setProperty("--p", progress);
  p.value = progress;

  corners.forEach((corner) => {
    if (progress > corner.st && progress < corner.ed) {
      showCorner.value = true;
      cornerStart.value = corner.st;
      cornerEnd.value = corner.ed;
      currentCorner.value = corner;
    }
  });

  sections.forEach((section) => {
    if (progress > section.st && progress < section.ed) {
      showSection.value = true;
      sectionStart.value = section.st;
      sectionEnd.value = section.ed;
    }
  });
}

function handleScroll() {
  if (window.scrollY > 2) {
    document.body.classList.add("scrolled");
  } else {
    document.body.classList.remove("scrolled");
  }
  updateScrollDistance();
}

function updatePageHeight() {
  const body = document.querySelector("body");
  if (window.innerHeight < window.innerWidth) {
    body.classList.remove("vertical");
    body.classList.add("horizontal");
  } else {
    body.classList.remove("horizontal");
    body.classList.add("vertical");
  }
}

// Lifecycle
onMounted(() => {
  const root = document.querySelector(":root");
  if (darkMode.value) {
    root.classList.add("dark");
  }

  window.addEventListener("scroll", handleScroll);
  window.addEventListener("resize", () => {
    updateScrollDistance();
    updatePageHeight();
  });

  updateScrollDistance();
  updatePageHeight();
});

onUnmounted(() => {
  window.removeEventListener("scroll", handleScroll);
  window.removeEventListener("resize", () => {
    updateScrollDistance();
    updatePageHeight();
  });
});
</script>
