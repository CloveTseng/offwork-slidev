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

等一下會帶大家參觀我們的開發成果以及整個流程

然後是我們使用的技術

還有之中
 -->
---
layout: two-cols
title: 開發成果流程導覽
---

<h2 class="font-extrabold text-[#A4CD44]">先來看我們的開發成果</h2>
<a href="https://offwork.clovetseng.dev/" target="_blank">https://offwork.clovetseng.dev/</a>

::right::

<Transform :scale="0.6">
<iframe src="https://offwork.clovetseng.dev/" width="375px" height="812px" class="border"></iframe>
</Transform>

<style>
  .border {
    border: 2px solid #A4CD44;
    border-radius: 16px;
  }
</style>
---
layout: center
title: 開發使用的技術
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
      <tr v-click>
        <td class="border px-4 py-2">Nuxt 4</td>
        <td class="border px-4 py-2">切版、開路由、拆元件、切 Layout</td>
      </tr>
      <tr v-click>
        <td class="border px-4 py-2">Tailwind CSS</td>
        <td class="border px-4 py-2">CSS 框架，tailwind config 套用設計系統</td>
      </tr>
      <tr v-click>
        <td class="border px-4 py-2">sessionStorage</td>
        <td class="border px-4 py-2">紀錄大吼、呼吸時間與是否已放鬆（isRelieved）</td>
      </tr>
      <tr v-click>
        <td class="border px-4 py-2">GSAP</td>
        <td class="border px-4 py-2">分析頁面動畫</td>
      </tr>
      <tr v-click>
        <td class="border px-4 py-2">Nuxt Lottie</td>
        <td class="border px-4 py-2">大吼分貝動畫</td>
      </tr>
      <tr v-click>
        <td class="border px-4 py-2">git</td>
        <td class="border px-4 py-2">版本控制與 Vercel 部署</td>
      </tr>
      <tr v-click>
        <td class="border px-4 py-2">Slidev</td>
        <td class="border px-4 py-2">製作這份簡報</td>
      </tr>
    </tbody>
  </table>
  <img src="/images/structure.png" v-click.hide="[2, 3]" />

<!-- 
[click] 我們主要是使用 Nuxt 4 來進行開發，會選擇 Nuxt 的原因是因為能夠大量的簡化開發的流程，他可以自動化幫我們生成路由以及自動引入常見的 Vue API ，以及簡化許多環境設定的時間，讓我們可以專注在切版、拆分元件跟 layout 上面

[click] 我們 UI 的部份是使用 TailwindCSS 
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

---
title: 參加研發營的收穫與成長
---

<h1 class="font-extrabold text-[#A4CD44]">參加研發營的收穫與成長</h1>

<h2 class="font-bold">Aaron</h2>

很難得有機會能練習到像 AAPD 這種「非常規版面」的網站，在挑戰切版技巧的同時，對我來說也是一次很棒的經驗。

<h2 class="font-bold">Clove</h2>

收穫與成長...

<h2 class="font-bold">Tippy</h2>

收穫與成長...
