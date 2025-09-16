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
layout: center
title: 開發使用的技術
dragPos:
  foo: 653,132,325,_
  tailwind: 698,114,262,_
  after: 72,310,866,292
  charts: 617,270,237,145
  lottie: 560,240,171,253
---

<h1 class="font-extrabold text-[#A4CD44] text-center">開發使用的技術</h1>

  <table class="border-collapse">
    <thead>
      <tr>
        <th class="border px-4 py-2 text-left">技術</th>
        <th class="border px-4 py-2 text-left">說明</th>
      </tr>
    </thead>
    <tbody>
      <tr v-click="1">
        <td class="border px-4 py-2">Nuxt 4</td>
        <td class="border px-4 py-2">切版、開路由、拆元件、切 Layout</td>
      </tr>
      <tr v-click="2">
        <td class="border px-4 py-2">Tailwind CSS</td>
        <td class="border px-4 py-2">CSS 框架，tailwind config 套用設計系統</td>
      </tr>
      <tr v-click="3">
        <td class="border px-4 py-2">sessionStorage</td>
        <td class="border px-4 py-2">紀錄大吼、呼吸時間與是否已放鬆（isRelieved）</td>
      </tr>
      <tr v-click="4">
        <td class="border px-4 py-2">GSAP</td>
        <td class="border px-4 py-2">分析頁面圖表載入動畫</td>
      </tr>
      <tr v-click="5">
        <td class="border px-4 py-2">Nuxt Lottie</td>
        <td class="border px-4 py-2">大吼分貝動畫</td>
      </tr>
      <tr v-click="6">
        <td class="border px-4 py-2">git</td>
        <td class="border px-4 py-2">版本控制與 Vercel 部署</td>
      </tr>
      <tr v-click="7">
        <td class="border px-4 py-2">Slidev</td>
        <td class="border px-4 py-2">製作這份簡報</td>
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
  <img src="/images/after.png" v-drag="'after'" />
  </div>
  <div v-click="[4,5]">
  <img src="/images/charts.png" v-drag="'charts'" />
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
  aaron: 351,12,325,_
---

<h1 class="font-extrabold text-[#A4CD44]">開發中的亮點</h1>

<div class="flex">
  <img src="/images/avatar/Aaron.svg" width="50px" />
  <h4 v-click>Aaron：開營即結訓</h4>
</div>
<div v-click="[1,2]">
  <img src="/images/aaron-highlight.png" v-drag="'aaron'" />
</div>
<div class="flex">
  <img src="/images/avatar/Clove.svg" width="50px" />
  <h4 v-click>Clove：</h4>
</div>
<div class="flex">
  <img src="/images/avatar/Tippy.svg" width="50px" />
  <h4 v-click>Tippy：</h4>
</div>

<style>
  .flex {
    padding: 16px 0;
    display: flex;
    align-items: center;
    gap: 8px;
  }

</style>

<!--
Aaron：
開營即結訓

Clove：
開發中為自己感到驕傲的地方

Tippy：
開發中為自己感到驕傲的地方
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
  <img src="/images/analyze.png" v-drag="'analyze'" />
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
