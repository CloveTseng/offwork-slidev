---
layout: cover
highlighter: default
title: OFFWORK
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
<div v-click="[4,5]">
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
Aaron：
一開始在做「平穩呼吸法」呼吸練習頁面時，因為動畫效果比較少見又有點複雜，加上我對 mask 的用法也不太熟，所以卡了滿久。後來花了很多時間研究、問 GPT，才把問題解決。

Clove：
遇到的困難與解決方式...

Tippy：
遇到的困難與解決方式...
-->

---
title: 團隊協作、工作分配
dragPos:
  index: 341,148,157,308
  analyze: 505,149,160,310
  my: 678,148,162,310
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
  <img src="/images/analyze.webp" v-drag="'analyze'" />
</div>
<div v-click>
  <img src="/images/my.png" v-drag="'my'" />
</div>

<!--
這裡列出了我們整個開發的工作分配，主要分成

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
<p v-click>很難得有機會能練習到像 AAPD 這種「非常規版面」的網站，在挑戰切版技巧的同時，對我來說也是一次很棒的經驗。</p>

<div class="flex">
  <img src="/images/avatar/Clove.svg" width="50px" />
  <h2 class="font-bold">Clove</h2>
</div>
<p v-click>收穫與成長...</p>

<div class="flex">
  <img src="/images/avatar/Tippy.svg" width="50px" />
  <h2 class="font-bold">Tippy</h2>
</div>

<p v-click>收穫與成長...</p>

<style>
  .flex {
    display: flex
  }
  h2 {
    padding: 4px;
  }
  p {
    margin-bottom: 30px;
  }
</style>
<!-- 

 -->
---
layout: center 
hideInToc: true
---
# END
