---
layout: cover
title: OFFWORK
highlighter: shiki
favicon: "/favicon.ico"
fonts:
  sans: "Noto Sans TC"
  mono: "Fira Code"
transition: fade-out
hideInToc: true
---

<div class="flex flex-col items-center">
  <h1 class="font-extrabold text-[#A4CD44]">OFFWORK</h1>
  <p>丟掉煩惱，讓腦袋準時下班</p>
  <h3>AAPD x 六角學院成果展示</h3>
  <h5 v-click>設計組：</h5>
  <div>
  <span v-click> Jerry <img src="/images/avatar/Jerry.svg" width="50px" /> </span>
  <span v-after> Anna <img src="/images/avatar/Anna.svg" width="50px" /> </span>
  <span v-after> Alvie <img src="/images/avatar/Alvie.svg" width="50px" /> </span>
  <span v-after> Maggie <img src="/images/avatar/Maggie.svg" width="50px" /> </span>
  <span v-after> Oliver <img src="/images/avatar/Oliver.svg" width="50px" /> </span>
  <span v-after> Yien <img src="/images/avatar/Yien.svg" width="50px" /> </span>
  </div>
  <h5 v-click>前端組：</h5>
  <div>
  <span v-click> Aaron <img src="/images/avatar/Aaron.svg" width="50px" /> </span>
  <span v-click> Clove <img src="/images/avatar/Clove.svg" width="50px" /> </span>
  <span v-click> Tippy <img src="/images/avatar/Tippy.svg" width="50px" /> </span>
  </div>
</div>

<style>
  h3 {
    font-weight: 700;
    margin-bottom: 16px;
  }
  p {
    font-size: 14px;
  }
  h5 {
    margin-top: 16px;
  }
  div {
    display: flex;
  }
  span {
    text-align: center;
    padding: 8px;
    font-size: 16px;
  }
</style>

<!--
Hi, 大家好，我是 Clove，我們是 OFFWORK 

[click] 我們的設計組成員有以下這六位…，[click]

[click] 以及前端組的成員有我們捲佑哥

[click] 以及我本人

[click] 還有我們的 Tippy 前輩
-->

---
layout: two-cols
layoutClass: gap-16
---

# 簡報目錄

快速導覽到要展示的內容

<img src="/images/toc-deco.webp" alt="裝飾圖案" class="max-w-80" />

::right::

<Toc text-lg minDepth="1" maxDepth="2" />

<!--
接著是我們這次成發的簡報流程：

等一下會帶大家參觀我們的開發成果以及 APP的流程

然後是我們使用的技術及亮點

以及之中遇到的困難和解決方式

最後是收獲與成長
-->

---
layout: two-cols
title: 開發成果流程導覽
---

<h2 class="font-extrabold text-[#A4CD44]">先來看我們的開發成果</h2>
<a href="https://offwork.clovetseng.dev/" target="_blank">https://offwork.clovetseng.dev/</a>
<h6>丟掉煩惱，讓腦袋準時下班</h6>

::right::

<Transform :scale="0.6">
<iframe src="https://offwork.clovetseng.dev/" width="375px" height="812px" class="border"></iframe>
</Transform>

<style>
  .border {
    border: 2px solid #A4CD44;
    border-radius: 16px;
  }
  h2 {
    padding-bottom: 16px;
  }
</style>

<!--
先來看我們的發表成果：

這是我們這一次開發的健康生活 APP OFFWORK，

1. 首頁：下班的時候已經累積了許多壞心情，所以大家可以看到火山君都快爆發了，
2. 下班儀式：使用者可以從首頁的『下班儀式』來吼一吼、或是呼吸(點擊『先躺平』離開)
3. 我的：也可以從個人資料這裡開始下班儀式(點擊)，大家想先大吼還是先呼吸呀~
4. 首頁：大家可以看到現在火山君已經變成綠色火山君，心情已經好多了
5. 我的：可以從個人資訊這邊看到今天的活動紀錄
6. 在我的資訊這裡設定呼吸及睡眠的目標，以及開啟通知功能
6. 查看更多：然後查看更多可以有更詳細的分析資訊
7. (7/17)：也可以點選日期選擇其他天的資料
8. 大吼：或是查看每週、每月的更詳細數據
-->

---
layout: two-cols
title: 開發使用的技術
dragPos:
  foo: 536,76,418,_
  tailwind: 555,12,355,_
  after: 509,161,559,327
  charts: 593,251,293,179
  lottie: 603,131,243,360
---

<h2 class="font-extrabold text-[#A4CD44] text-center pb-2">開發使用的技術</h2>

  <table class="border-collapse">
    <thead>
      <tr>
        <th class="border px-4 py-1 text-left">技術</th>
        <th class="border px-4 py-1 text-left">說明</th>
      </tr>
    </thead>
    <tbody>
      <tr v-click="1">
        <td class="border px-4 py-1">Nuxt 4</td>
        <td class="border px-4 py-1">切版、開路由、拆元件、切 Layout</td>
      </tr>
      <tr v-click="2">
        <td class="border px-4 py-1">Tailwind CSS</td>
        <td class="border px-4 py-1">CSS 框架，tailwind config 套用設計系統</td>
      </tr>
      <tr v-click="3">
        <td class="border px-4 py-1">sessionStorage</td>
        <td class="border px-4 py-1">紀錄大吼、呼吸時間與是否已放鬆（isRelieved）</td>
      </tr>
      <tr v-click="4">
        <td class="border px-4 py-1">GSAP</td>
        <td class="border px-4 py-1">分析頁面圖表載入動畫</td>
      </tr>
      <tr v-click="5">
        <td class="border px-4 py-1">Nuxt Lottie</td>
        <td class="border px-4 py-1">大吼分貝動畫</td>
      </tr>
      <tr v-click="6">
        <td class="border px-4 py-1">git</td>
        <td class="border px-4 py-1">版本控制與 Vercel 部署</td>
      </tr>
      <tr v-click="7">
        <td class="border px-4 py-1">Slidev</td>
        <td class="border px-4 py-1">製作這份簡報</td>
      </tr>
    </tbody>
  </table>
  <div v-click="[1,2]">
    <img src="/images/structure.png" v-drag="'foo'" />
  </div>
  <div v-click="[2,3]">
  <img src="/images/tailwind-config.png" v-drag="'tailwind'" />
  </div>
  <div v-click="[3,4]">
  <img src="/images/after.webp" v-drag="'after'" />
  </div>
  <div v-click="[4,5]">
  <img src="/images/charts.webp" v-drag="'charts'" />
  </div>
  <div v-click="[5,6]">
  <img src="/images/lottie.png" v-drag="'lottie'" />
  </div>

<!--
[click] 我們主要是使用 Nuxt 4 來進行開發，會選擇 Nuxt 的原因是因為能夠大量的簡化開發的流程，他可以自動化幫我們生成路由以及自動引入常見的 Vue API ，以及簡化許多環境設定的時間，讓我們可以專注在切版、拆分元件跟 layout 上面

[click] 在 UI 的部份我們是使用 TailwindCSS，除了能直接在 class 撰寫樣式，省去額外寫 css 的步驟，我們還在 `tailwind.config` 中套用設計系統，能統一風格並且也加速開發效率

[click] 在呼吸或大吼之後，就會把資訊存在 sessionStorage 裡面，`isRelieved` 從 false 改為 true ，並且紀錄大吼的秒數

[click] 圖表載入時的動畫則是使用了 GSAP 來處理

[click] 在大吼的動畫我們使用了 lottie 大吼的動畫

[click] 最後是使用 git 來進行版本控作及協作，並且部署到 vercel 上
-->

---
title: 開發中的亮點
dragPos:
  aaron: 479,12,325,_
  highlight-1: 436,140,416,87
  highlight-meta: 437,226,392,180
  highlight-clock: 458,195,403,105
  highlight-3: 371,148,588,315
---

<h1 class="font-extrabold text-[#A4CD44]">開發中的亮點</h1>
<div class="flex">
  <img src="/images/avatar/Aaron.svg" width="50px" />
  <img src="/images/avatar/Clove.svg" width="50px" />
  <img src="/images/avatar/Tippy.svg" width="50px" />
</div>
<v-clicks>
  <li>捲佑哥的『開營即結訓』風雲</li>
  <li>高手在乎細節</li>
  <li>https://offwork.clovetseng.dev</li>
  <li>不只是開發，也注重效能</li>
</v-clicks>
<div v-click="[1,2]">
  <img src="/images/aaron-highlight.webp" v-drag="'aaron'" />
</div>
<div v-click="[2,3]">
  <img src="/images/highlight-1.png" v-drag="'highlight-1'" />
  <img src="/images/highlight-meta.png" v-drag="'highlight-meta'" />
</div>
<div v-click="[3,4]">
  <img src="/images/highlight-clock.png" v-drag="'highlight-clock'" />
</div>
<div v-click="4">
  <img src="/images/highlight-3.png" v-drag="'highlight-3'" />
</div>

<style>
  .flex {
    display: flex;
    margin-bottom: 16px;
  }
  img {
    padding: 2px;
  }

</style>

<!--
接著想要介紹我們專題中的亮點：

[click] 捲佑哥的開營即結訓風雲，開營當天被發現已經做完了初切版，並且也因為這一波，今年很多組別都套了手機框，一年成發比一年高級ww 不是說好的切版嗎…

[click] 過去在拿到設計稿後，我通常會直接進入開發階段。思考佈局、拆分元件、定義變數，然後開始選擇適合的技術來實現，

但這次，在完成環境設定後，參考了捲哥的切版作業，第一次花時間去研究並撰寫 meta tags，這些看似不起眼的小事情，卻會大大提升整個專案對於 SEO 及社群媒體的分享，

[click] 以及就算是手機模擬框，也要插一個真的時鐘在這裡的小細節(可以到網站去看)

[click] 這是 google 的網站 pagespeed 測試出來的結果，過去開發時我們專注在把東西做出來，這次注重網站除了完整，也要跑得流暢，例如將圖片進行壓縮及將 png 轉成更輕量的 WebP 格式
-->

---
layout: center
title: 開發過程遇到的困難與解決方式
---

<h1 class="font-extrabold text-[#A4CD44]">開發過程遇到的困難與解決方式...</h1>

<!--
接下來說明一下我們在開發時遇到的困難及解決辦法
-->

---
layout: two-cols
title: Aaron 的困難與解決
hideInToc: true
---

<h2>Aaron - 困難與解決方式</h2>
<ul>
  <li>動畫效果</li>
</ul>

::right::

<Transform :scale="0.6">
<iframe src="https://offwork.clovetseng.dev/find-peace/calm-breathe" width="375px" height="812px" class="border"></iframe>
</Transform>

<style>
.border {
  border: 2px solid #A4CD44;
  border-radius: 16px;
}
h2 {
  padding-bottom: 16px;
}
</style>

<!-- 
Aaron：
一開始在做「平穩呼吸法」呼吸練習頁面時，因為動畫效果比較少見又有點複雜，加上我對 mask 的用法也不太熟，所以卡了滿久。後來花了很多時間研究、問 GPT，才把問題解決。 
-->
---
title: Tippy 的困難與解決
hideInToc: true
---
<h2>Tippy - 困難與解決方式</h2>

<div class="flex gap-5">
<div>

1. scrollbar 資料的無限循環 - [無限滾動時間軸筆記](https://hackmd.io/@sGWlDvZ7Q8S1PeDHFopP9w/rJUNMjf9xe#無限滾動時間軸)

<div class="flex gap-4 mb-2">
  <img src="/images/timeScrollbar.png" width="150px" />
<img src="/images/notifyScrollbar.png" width="150px" />

</div>
<iframe height="300" style="width: 100%;" scrolling="no" title="無限滾動時間軸" src="https://codepen.io/Ektodor-Wang/embed/qEOJNZz?default-tab=result" frameborder="no" loading="lazy" allowtransparency="true" allowfullscreen="true">
</iframe>
  </div>
<br>

<div>

2. 火山君離開視線後觸發特定樣式

- 使用 `IntersectionObserver(callback,[option])`
<div class="flex gap-4 mb-2">
  <img src="/images/my-1.png" width="200px" />
<img src="/images/my-2.png" width="200px" />

</div>
</div>

</div>

<style>
h2 {
  padding-bottom: 16px;
}
</style>

<!--
Tippy：
在這次切版過程中，遇到了一些以往沒有實作過的特殊樣式和互動情境，例如 scrollbar 資料的無限循環，以及火山君離開視線後觸發特定樣式的設計。這些需求對我來說都是全新的挑戰，一開始在實作時卡關了好一陣子。只要當我卡了一段時間後，我通常會去請教 Claude。雖然他給的程式碼不一定能直接執行，但他提供的解法邏輯與思路能幫我打開新的方向。
-->

---
layout: two-cols
title: Clove 的困難與解決
hideInToc: true
dragPos:
  foo: 819,194,62,_,31
---

<h2>Clove - 困難與解決方式</h2>
<ul>
  <li v-click="1"> Vue3 還不會就要直上 Nuxt 太刺激了吧!!!</li>
  <li v-click="5">元件傳值傳好傳滿</li>
</ul>


::right::

<img v-click="2" src="/images/clove-difficulty-1.png" />
<img v-click="2" src="/images/clove-difficulty-2.png" />
<img v-click="3" src="/images/clove-difficulty-3.png" />

<div v-click="4">
  <img src="/images/clove-1.svg" v-drag="'foo'" />
</div>

```js {hide|hide|hide|hide|hide|hide|1,3|5-8}
// 父元件
<div v-if="!chartData" class="text-xs text-neutral-300 py-2">資料載入中…</div>
<ChartsTimelineChart v-else :chart-data="chartData" />

// 子元件
const props = defineProps({
  chartData: {
    type: Object,
    required: true,
  }
});
```

<style>
h2 {
  padding-bottom: 16px;
}
img {
  margin-top: 4px;
}
li {
  margin-bottom: 140px
}
</style>

<!--
[click]
 在捲佑哥發現我們同一組的時候，就跑來問我說：[click] 你會 vue 嗎？當時我剛開始 vue 的新手營不久，就是一腦子可以的吧行的吧!

[click] 捲哥就回我：那我們就用 nuxt + tailwind 來開發，
[click] 所以我新手營上的特別特別的認真

[click] 再來我必須說我在之前 React 班的時候傳值真心沒學好，導致我拆元件後元件一多的狀況下，對於資料的流動和管理總是感到很混亂。

[click] 所以這次認真去學習 Vue 的傳值方式也會重新反思當時專題時 React 的寫法是不是可以更好，並且去深入理解如何讓資料流向變得清晰、可追溯
-->

---
title: 團隊協作、工作分配
dragPos:
  index: 361,151,157,308
  analyze: 537,152,157,308
  my: 710,152,157,308
---

<h1 class="font-extrabold text-[#A4CD44]">團隊協作、工作分配</h1>

<h2 class="font-bold">Aaron</h2>

<ul class="text-xs">
 <li>首頁兩種狀態&下班儀式流程</li>
 <li>Bottom Sheet、Modal 元件製作</li>
 <li>手機外框 Layout 製作（特別感謝 Barry）</li>
</ul>

<h2 class="font-bold">Clove</h2>

<ul class="text-xs">
 <li>分析頁面&流程</li>
 <li>GSAP 動畫</li>
 <li>使用 ECharts 來處理圖表</li>
</ul>

<h2 class="font-bold">Tippy</h2>

<ul class="text-xs">
 <li>我的頁面&流程</li>
 <li>時間捲動元件</li>
</ul>

<div v-click>
  <img src="/images/index.png" v-drag="'index'" />
</div>
<div v-click>
  <img src="/images/analyze.png" v-drag="'analyze'" />
</div>
<div v-click>
  <img src="/images/my.png" v-drag="'my'" />
</div>

<!--
接著，這裡列出了我們整個開發的工作分配，主要分成

[click]首頁

[click]分析頁

[click]我的頁面三個大塊，然後再細分功能與流程
-->

---
title: 參加研發營的收穫與成長
---

<h1 class="font-extrabold text-[#A4CD44]">參加研發營的收穫與成長</h1>

<div class="flex">
  <img src="/images/avatar/Aaron.svg" width="50px" />
  <h2 class="font-bold">Aaron</h2>
</div>
<ul v-click class="mb-30">
  <li>有機會開發「非常規版面」的網站</li>
  <li>手機框及動畫很好玩</li>
</ul>

<div class="flex">
  <img src="/images/avatar/Clove.svg" width="50px" />
  <h2 class="font-bold">Clove</h2>
</div>
<ul v-click class="mb-30">
  <li>學習並實戰 Vue3 + Nuxt 框架</li>
  <li>細節思維</li>
  <li>多了很多面試機會(?)</li>
</ul>

<div class="flex">
  <img src="/images/avatar/Tippy.svg" width="50px" />
  <h2 class="font-bold">Tippy</h2>
</div>

<div v-click class="mb-30">
<ul>
<li>切版技巧與 Nuxt 框架</li>
<li>設計師與工程師的協作模式</li>
<li>認識超捲超carry的組員🤣</li>
</ul>
</div>

<style>
  .flex {
    display: flex
  }
  h2 {
    padding: 4px;
  }
  .mb-30 {
    margin-bottom: 20px;
  }
</style>

<!--
[click] Aaron：很難得有機會開發到這種非常規的版面，實作了一些平常工作中不常使用到的技術，在挑戰切版技巧的同時，對我來說也是一次很棒的經驗。

[click] Clove : 本來參加研發營，只是想著多一份作品，但意外的收獲是多了一個 Nuxt.js (Vue3) 的實戰開發經驗。更重要的是從單純寫程式的工程師轉變為一個思考架構、注重細節的工程師。
明年沒意外的話，還會再看到我的出現，期待又是一個不同的成長與經歷。

[click] Tippy : 這次參與 AAPD 的活動，除了練習切版技巧與 Nuxt 框架的應用外，最重要的收穫是更深入地了解了設計師與工程師之間的協作模式。其中，讓我最意想不到的收穫是在這段過程中認識了墨和捲佑，與他們一起開發的時候是會被他們的積極性給影響的（畢竟捲神開營即結訓）。雖然這樣的節奏多少會帶來一些壓力，但那是一種良性的推動力（大家一起捲起來～～）。這次的經歷，也許不是技術層面的飛躍，卻是我在心態上非常寶貴的一次成長。
-->

---
layout: center
hideInToc: true
---

# END
