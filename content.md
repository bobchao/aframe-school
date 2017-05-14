<!-- Title slide. -->
<!-- .slide: data-background="media/img/aframe.jpg" -->

<div class="talk-title">
  <h1>A-Frame 學院</h1>
  <h3>WebVR 的互動式學習教材</h3>
  <p class="talk-info">
    <b><a href="https://aframe.io">aframe.io</a></b>
  </p>
</div>

------

## 序章

<!-- .slide: data-background="media/img/aframe.jpg" -->

> 此教材將以 Step-by-step 的方式，透過 [Glitch](https://glitch.com) 練習，
> 協助您快速進入 [WebVR](https://webvr.rocks) 的世界！  
> 除了 &larr; 與 &rarr; 之外，這份教材裡也有 **&uarr; 及 &darr;** 的各節內容：

<img class="stretch" data-src="media/img/navigation.jpg">

**繼續往 &darr; 瀏覽**

---

### 旅途中的各種實用資源

1. [閱讀文件及 FAQ](https://aframe.io/docs/)
2. [到 Slack 尋求同好協助](https://aframe.io/community/#slack)
3. [在 Stack Overflow 上發問](http://stackoverflow.com/questions/ask/?tags=aframe)
4. 如果您正在參與工作坊，有問題就直接舉手吧！

**繼續往 &rarr; 瀏覽**


<!-- Lessons start below. -->


------

## Glitch &mdash; 介紹

> 此教材使用 [Glitch](https://glitch.com) 作為 A-Frame 的教學用開發環境。

<img class="stretch" data-src="media/img/glitch.jpg">

- Glitch 讓你可以在瀏覽器裡直接編寫程式，什麼也不必安裝設定
- Glitch 讓你可以**重混**別人已經寫好的 A-Frame 專案，不必從零開始
- Glitch 可以存放你的作品，並即刻透過網址（像是 `https://aframe.glitch.me`）發佈
- Glitch 可以在你更動 A-Frame 專案網站的程式碼時自動更新
- Glitch 可以讓很多人共同編輯同一個專案

*如果你想要自己設定本機開發環境，&darr; 面有相關說明*

---

## Glitch &mdash; 重混既有專案

> 你可以在 Glitch 上重混或 fork 既有的專案，以別人做好的東西為新專案的起點。
> 在開始之前，我們推薦你先將 Glitch 與 [GitHub 帳號](https://github.com/)連結。
> 編寫完畢後，Glitch 會隨機提供一個網址，這個網址可以進一步修改。

<img class="stretch" data-src="media/img/glitch2.jpg">

[在 Glitch 上重混 A-Frame 新手起步專案](https://glitch.com/~aframe/)  <!-- .element: class="cta-button glitch" -->

---

## Glitch &mdash; 編寫程式

> 在[重混 A-Frame 新手起步專案](https://glitch.com/~aframe/)後，咱們好好看看這個
> 編寫程式的地方。你還可以修改後端程式、上傳素材、建立新檔，甚至邀請其他人跟你一起寫程式！

<img class="stretch" data-src="media/img/glitch3.jpg">

---

## Glitch &mdash; 檢視專案成果

> 看完編輯畫面後，我們來看看專案的成果畫面。

<img class="stretch" data-src="media/img/glitch4.jpg">

---

## Glitch &mdash; 匯出專案

> 如果你想要下載整個專案的文件，或將專案匯出到 GitHub，請到專案選單裡的 *Advanced Options*。
> 點選 *Download Project* 後會給你一個 `.tgz` 檔，可以拿 ZIP 工具解開取得專案檔案。
> 對於 A-Frame 專案來說，你想要的東西都會在 `public/` 資料夾中，而後端的程式檔案都可以不管。

<img class="stretch" data-src="media/img/glitch5.jpg">

在下載專案後，如果你想要在自己的電腦上設定 Web 開發環境，那就請繼續往 **&darr;** 看；  
不然，就直接往 **&rarr;** 來開始 A-Frame 之旅吧！

---

## [非必備] 設定本機的 Web 開發環境

> 你可以在自己的電腦上設定完整的 Web 開發環境，不見得要仰賴 Glitch 的線上系統。

<img class="stretch" data-src="media/img/webdevenv1.jpg">

1. **挑個文字編輯器：** 拿 [Atom](https://atom.io) 作為入門還不錯
2. **安裝本機的伺服器：** 您可下載 [Mongoose
Server](https://www.cesanta.com/products/binary)，或在終端機中輸入 `python -m
SimpleHTTPServer`
3. **建立 `index.html` 檔**後複製 Glitch 範例裡的 A-Frame 程式碼過去
4. 在 HTML 檔的同一個目錄下**執行本機伺服器**
5. 在瀏覽器中**開啟本機伺服器的 URL**（例如 `http://localhost:8000`）
6. **修改 HTML 檔**，然後重新讀取網頁來檢視調整結果
7. 選配：可以考慮使用 [ngrok](https://ngrok.io) 來讓其他網段的任何設備都能存取本機伺服器

---

## [非必備] 設定本機的 Web 開發環境 &mdash; 挑個文字編輯器

> 如果你還沒有慣用的文字編輯器，[Atom](https://atom.io) 滿適合新手的。
> 其他熱門的選項還包括 [Notepad++](https://notepad-plus-plus.org/)、
> [Sublime](https://www.sublimetext.com/)、[Brackets](http://brackets.io/)以及
> [vim](http://www.vim.org/download.php) 等。

<img class="stretch" data-src="media/img/webdevenv2.jpg">

---

## [非必備] 設定本機的 Web 開發環境 &mdash; 安裝本機的伺服器

> 你會需要在本機安裝 HTTP 伺服器，以便將檔案送到瀏覽器.

<div class="captioned-image-row small">
  <div>
    <img data-src="https://cloud.githubusercontent.com/assets/8731271/24021623/10654d22-0a5f-11e7-9769-63cdff91637c.png">
    <a href="https://www.cesanta.com/products/binary">Mongoose Binary</a>
  </div>
  <div>
    <img data-src="https://www.python.org/static/opengraph-icon-200x200.png">
    <code>python -m SimpleHTTPServer 8080</code>
  </div>
  <div>
    <img data-src="https://www.echosteg.com/images/blog/standard/nodejs_logo.png">
    <a href="https://docs.npmjs.com/getting-started/installing-node">Node + npm + live-server</a>
  </div>
</div>

---

## [非必備] 設定本機的 Web 開發環境 &mdash; 使用 ngrok

> 你也可以考慮使用 [ngrok](https://ngrok.com/)，在不用瞎搞 IP 位置的情況下方便
> 於開發給手機使用的 A-Frame 專案。

1. 下載並解壓縮 [ngrok](https://ngrok.com/download/)
2. 執行 ngrok，提供本機伺服器的通訊埠號（例如 `./ngrok http 8080`）
3. 執行後，ngrok 會提供一串 URL 給你，例如 `https://abcdef123456.ngrok.io`
4. 接著就可以在任何網段、任何設備上開啟這個 URL，存取本機伺服器資源了

<img class="stretch" data-src="media/img/webdevenv3.jpg">

------

## 試試 A-Frame 的範例

> 在桌機或手機上打開 [A-Frame 的首頁](https://aframe.io)、
> [A-Frame 網誌](https://aframe.io/blog/) 或
> [awesome-aframe](https://github.com/aframevr/awesome-aframe)。  
> 如果你有頭戴型顯示器，請參考 [webvr.rocks](https://webvr.rocks) 來設定 WebVR。

<img data-src="media/img/examples.gif">

------

## 就從 *Hello, WebVR* 開始

> A-Frame 為初學者提供了一些容易使用的 HTML 元素，
> 我們稱之為 [基本型（primitive）](https://aframe.io/docs/0.5.0/primitives/)。
> 在下一節裡，我們會藉由調整 HTML 屬性方式來修改些東西（像是改顏色、位置、旋轉、大小等等），
> 感受一下整體作業流程。

<img data-src="media/img/hellowebvr2.jpg">

<img class="stretch" data-src="media/img/hellowebvr.jpg">

---

## 就從 *Hello, WebVR* 開始 &mdash; 位置（Position）

> `position` 定義了物件在 3D 環境的位置（有 X、Y、Z 三個方向軸），單位為公尺。
> 修改 `position` 這個 HTML 屬性值即可，詳情可[參考
> position 組件的說明](https://aframe.io/docs/master/components/position.html)。

[在 Glitch 上重混這一課的程式碼](https://glitch.com/~aframe-school-position)  <!-- .element: class="cta-button glitch" -->

1. *減少* `position` 屬性的 X 值，以便將圓柱體（cylinder）向左移
2. *增加* `position` 屬性的 Y 值，以便將正方體（box）向上移
3. *減少* `position` 屬性的 Z 值，以便將球體（sphere）向後移
4. **加分題：** 在 `<a-sphere>` 中加上一個子元素  `<a-ring>`，賦予位置設定後來看看他們之間的相對關係

<img class="stretch" data-src="media/img/positionresult.jpg">

[檢視最後成果](https://aframe-school-position.glitch.me/solution.html)  <!-- .element: class="cta-button" -->

---

## 就從 *Hello, WebVR* 開始 &mdash; 旋轉（Rotation）

> `rotation` 定義了物件在 3D 環境的旋轉角度（三個值分別為 X、Y、Z 三軸的旋轉角度），單位為度。
> 旋轉時依據右手定律來看角度，詳情可[參考
> rotation 組件的說明](https://aframe.io/docs/master/components/rotation.html)。

[在 Glitch 上重混這一課的程式碼](https://glitch.com/~aframe-school-rotation)  <!-- .element: class="cta-button glitch" -->

1. 調整圓柱體（cylinder）的 X 軸旋轉角度，以便秀出圓柱的底
2. 調整正方體（box）的 Y 軸旋轉角度，讓正面朝向鏡頭
3. **加分題：** 將整個場景的內容用 `<a-entity>` 包起來（作用就像 `<div>` 一般），接著調整其旋轉角度，查看個物件的相對旋轉方式

<img class="stretch" data-src="media/img/rotationresult.jpg">

[檢視最後成果](https://aframe-school-rotation.glitch.me/solution.html)  <!-- .element: class="cta-button" -->

---

## 就從 *Hello, WebVR* 開始 &mdash; 增加其他基本型

> 在 `<a-scene>` 裡可以加入其他 HTML 元素，並藉此添增其他基本型。
> [可參考基本型的相關說明](https://aframe.io/docs/0.5.0/primitives/)。

[在 Glitch 上重混這一課的程式碼](https://glitch.com/~aframe-school-primitives)  <!-- .element: class="cta-button glitch" -->

1. 在左側加上 [`<a-torus-knot>`](https://aframe.io/docs/0.5.0/primitives/a-torus-knot.html)
2. 在右側加上 [`<a-dodecahedron>`](https://aframe.io/docs/0.5.0/primitives/a-dodecahedron.html)
3. 於畫面中間加入 [`<a-text>`](https://aframe.io/docs/0.5.0/primitives/a-text.html)

<img class="stretch" data-src="https://cloud.githubusercontent.com/assets/674727/24266010/9c57cbe4-0fc2-11e7-968f-168f3649d109.png">

[檢視最後成果](https://aframe-school-primitives.glitch.me/solution.html)  <!-- .element: class="cta-button" -->

------

## 添加材質 &mdash; 上傳素材

> 接著我們要為這些物件添加一些圖片材質，看起來會比單純的色彩還讚。[你可以在網路上找一些圖
> 片](https://aframe.io/docs/0.5.0/introduction/faq.html#where-can-i-find-assets)，
> 然後上傳到 Glitch 的 assets 區或 [cdn.aframe.io](https://cdn.aframe.io)。
> 不管你要傳到哪裡，都記得要透過 HTTPS 傳輸，也要留意
> [CORS](https://developer.mozilla.org/docs/Web/HTTP/Access_control_CORS) 問題。

<img class="stretch" data-src="media/img/glitchasset.jpg">

接下來在本課程的 Glitch 中 **&darr;**，上圖所列出的素材已經先幫你傳到 assets 裡了。

---

## 添加材質 &mdash; 圖片材質

> 在 HTML 的 `src` 屬性裡填上圖片的 URL。[請參考將圖片設定為材質的
> 相關說明](https://aframe.io/docs/0.5.0/guides/#applying-an-image-texture)。

[在 Glitch 上重混這一課的程式碼](https://glitch.com/~aframe-school-textures/)  <!-- .element: class="cta-button glitch" -->

1. 為地板 `<a-plane>` 設定圖片材質
2. 為每個 `<a-box>` 設定圖片材質
3. 為 `<a-sphere>` 設定圖片材質
4. 為 `<a-cone>` 設定圖片材質
5. 為背景 `<a-sky>` 設定圖片材質，可上 [Flickr 的 360&deg; 照片群組](https://www.flickr.com/groups/equirectangular/) 找尋適當圖片。

<img class="stretch" data-src="media/img/texture.jpg">

[檢視最後成果](https://aframe-school-textures.glitch.me/solution.html)  <!-- .element: class="cta-button" -->

------

## 開啟 A-Frame Inspector

> 在**任何** A-Frame 場景中，你都可以按下 **`<ctrl> + <alt> + i`** 來開啟視覺化編輯器，
> 就跟瀏覽器的開發工具一樣！你可以到[首頁的範例集](https://aframe.io/examples/)裡挑幾個來試試，
> 也請參考 Inspector 相關說明](https://aframe.io/docs/master/guides/using-the-aframe-inspector.html)。

<img class="stretch" data-src="media/img/inspector.gif">

---

## 開啟 A-Frame Inspector &mdash; 調整組件設定值

> 在右側面板可以調整各實體上的組件設定值，藉此改變實體的外貌或行為。
> Inspector 可以辨識出所有 A-Frame 的組件，即使是社群提供的組件亦不例外。
> 此範例裡有個由社群撰寫的 [text-geometry 組件](https://www.npmjs.com/package/aframe-text-geometry-component)，
> Inspector 也能正確修改其設定值。

[到 Glitch 開啟這一課的範例](https://aframe-vaporwave.glitch.me)  <!-- .element: class="cta-button glitch" -->

1. 選定範例中的某個實體
2. 修改其 [`text-geometry` 組件](https://www.npmjs.com/package/aframe-text-geometry-component) 的 `value` 值

<img class="stretch" data-src="media/img/inspectorchange.jpg">

---

## 開啟 A-Frame Inspector &mdash; 加入 Registry 目錄中的組件

> 從 [Registry](https://aframe.io/registry/) 中可以
> 找到 [physics 組件](https://github.com/donmccurdy/aframe-physics-system)，
> 並且直接套用在當前場景中的實體上。
> Registry 是編排過的 A-Frame 組件集，而 Inspector 可整合 Registry，直接在實體面板中套用 Registry 收錄的組件。

[到 Glitch 開啟這一課的範例](https://aframe-vaporwave.glitch.me)  <!-- .element: class="cta-button glitch" -->

1. 為地板加上 `static-body` 組件
2. 為麻花結（後面那個紫色的東西）加上 `dynamic-body` 組件
3. 提升麻花結的 Y-position 值，使其位置升高
4. 離開 Inspector

<img class="stretch" data-src="media/img/inspectorregistry.gif">

------

## 以實體及組件編排場景內容 &mdash; 解構基本型

> 在那些好用的基本型之下，A-Frame 採用的是實體-組件的架構。我們回頭看一下
> *Hello, WebVR* 範例，並且嘗試將內容都解構為 `<a-entity>` 及其基礎組件。

[在 Glitch 上重混這一課的程式碼](https://glitch.com/~aframe-school-ecs)  <!-- .element: class="cta-button glitch" -->

[geometry]: https://aframe.io/docs/0.5.0/components/geometry.html
[material]: https://aframe.io/docs/0.5.0/components/material.html

1. 將 `<a-box>` 代換為擁有 [geometry][geometry] 及 [material][material] 組件的 `<a-entity>`，並設定 geometry 組件為 `primitive: box`
2. 將 `<a-sphere>` 代換為擁有 [geometry][geometry] 及 [material][material] 組件的 `<a-entity>`，並設定 geometry 組件為 `primitive: sphere`
3. 將 `<a-cylinder>` 代換為擁有 [geometry][geometry] 及 [material][material] 組件的 `<a-entity>`，並設定 geometry 組件為 `primitive: cylinder`
4. 將 `<a-plane>` 代換為擁有 [geometry][geometry] 及 [material][material] 組件的 `<a-entity>`，並設定 geometry 組件為 `primitive: plane`
5. 將 `<a-sky>` 代換為擁有 [geometry][geometry] 及 [material][material] 組件的 `<a-entity>`，並設定 geometry 組件為 `primitive: sphere` 加上 `radius: 3000`。隨後將 material 組件設定為 `shader: flat`，因為我們只需要單色，就不要花時間來計算光線效果了

[檢視最後成果](https://aframe-school-ecs.glitch.me/solution.html)  <!-- .element: class="cta-button" -->

---

## 以實體及組件編排場景內容 &mdash; 添增點光源

> 我們要使用實體及組件的模式，新增一個圓體並令其成為點光源。
> 要新增這樣的實體，必須混用 geometry、material 及 light 組件。

1. 找到 `<a-entity id="lightSphere">`
2. 加上 [geometry 組件](https://aframe.io/docs/0.5.0/components/geometry.html)，並設定為 `primitive: sphere`
3. 加上 [material 組件](https://aframe.io/docs/0.5.0/components/material.html)，並設定為 `color: #FFF` 及 `shader: flat`
4. 加上 [light 組件](https://aframe.io/docs/0.5.0/components/light.html)，並設定為 `type: point`
5. **加分題：** 透過 `<script>` 標籤從 [Registry](https://aframe.io/registry/) 為該實體加上 animation 組件，並設定 `property: position`、`dir: alternate` 及 `loop: true`，且用 `to: <POSITION>` 設定移動目的位置（x y z）。

[在 Glitch 上重混這一課的程式碼](https://glitch.com/~aframe-school-ecs-light-sphere)  <!-- .element: class="cta-button glitch" -->

<img class="stretch" data-src="https://cloud.githubusercontent.com/assets/674727/24060160/2c53a604-0b0f-11e7-9386-f83a3a9b4cfc.gif">>

[檢視最後成果](https://aframe-school-ecs-light-sphere.glitch.me/solution.html)  <!-- .element class="cta-button" -->

------

## 以 Registry 擴充實體及組件

> [Registry 網站](https://aframe.io/registry/)是尋找社群組件的好去處，
> 就像是所謂的外掛模組一樣能為 A-Frame 加強功能。只要從 Registry 找到適當的組件、
> 複製其 JS 連結、再透過 `<script>` 引入檔案中就可直接在 HTML 裡使用。

1. 先加入 [Particle
System](https://www.npmjs.com/package/aframe-particle-system-component) 組件，為每個
`<a-entity>` 加上 `particle-system` 屬性後設定為 `preset: default` 與 `preset: snow`，
接著開啟 Inspector 看看效果、調整屬性！
2. 加入 [Animation](https://www.npmjs.com/package/aframe-animation-component) 組件，
為球體套用縮放的動畫效果：加上 `animation` 屬性，並設定 `property: scale`、`loop: true`
及 `to: 1.1 1.1 1.1`
3. 以 `<script>`加入 [Outline Effect](https://www.npmjs.com/package/aframe-outline-effect) 組件後，在場景加上 `outline` 試試。

[在 Glitch 上重混這一課的程式碼](https://glitch.com/~aframe-school-registry)  <!-- .element: class="cta-button glitch" -->

<img class="stretch" data-src="media/img/registryexample.gif">

[檢視最後成果](https://aframe-school-registry.glitch.me/solution.html)  <!-- .element class="cta-button" -->

------

## 使用 JavaScript

> 你可以使用 JavaScript 與 DOM API 來用程式操作、修改實體。A-Frame 不只能玩 HTML，更能透過
> JavaScript、DOM API 及 three.js 發揮完整威力。[請參閱 *Using JavaScript and DOM
> APIs* with A-Frame](https://aframe.io/docs/0.5.0/guides/using-javascript-and-dom-apis.html)
> 一文。

[在 Glitch 上重混這一課的程式碼](https://glitch.com/~aframe-school-js)  <!-- .element: class="cta-button glitch" -->

<img class="stretch" data-src="media/img/js.jpg">

若想看見 JavaScript 的記錄資訊，可以在網頁上按右鍵，點擊*檢測元素*後，在瀏覽器的開發工具裡切換到*主控台*。
在檢視成果時，可以透過這個主控台來檢查內容。

---

## 使用 JavaScript &mdash; 取得實體

> 使用
> [`document.querySelector()`](https://developer.mozilla.org/docs/Web/API/Document/querySelector)
> 及
> [`document.querySelectorAll()`](https://developer.mozilla.org/docs/Web/API/Document/querySelectorAll)
> 取得場景及其中實體的參照。[請參閱查詢實體的相關文
> 件](https://aframe.io/docs/0.5.0/guides/using-javascript-and-dom-apis.html#getting-entities-by-querying-and-traversing).

[在 Glitch 上重混這一課的程式碼](https://glitch.com/~aframe-school-js)  <!-- .element: class="cta-button glitch" -->

1. 以 `var sceneEl = document.querySelector('a-scene');` 取得 `<a-scene>` 元素的參照
2. 以 `sceneEl.querySelectorAll('a-entity');` 取得所有 `<a-entity>` 元素的參照
3. 以 `sceneEl.querySelector('#box');` 取得該方塊的參照
4. 自己試試：用一次 `.querySelectorAll()` 搭配多元素選取符，取得球體跟圓柱體的參照
5. 自己試試：為球體跟圓柱體加上 class 後，用一次 `.querySelectorAll()` 取得他們的參照

[檢視最後成果](https://aframe-school-js.glitch.me/solution.html)  <!-- .element: class="cta-button" -->

---

## 使用 JavaScript &mdash; 調整實體設定

> 在上一節的練習後，現在我們使用取回的參照，進一步以
> [`Entity.setAttribute()`](https://aframe.io/docs/0.5.0/core/entity.html#setattribute-attr-value-componentattrvalue)
> 來修改實體內的屬性。[請參閱關於修改實體的相關文
> 件](https://aframe.io/docs/0.5.0/guides/using-javascript-and-dom-apis.html#modifying-an-entity)。

[在 Glitch 上重混這一課的程式碼](https://glitch.com/~aframe-school-js)  <!-- .element: class="cta-button glitch" -->

1. 試著調整正方體的 `rotation` 組件
2. 試著調整圓柱體的 `geometry` 組件之 `height` 屬性
3. 試著調整球體的 `material` 組件之 `metalness` 屬性

[檢視最後成果](https://aframe-school-js.glitch.me/solution2.html)  <!-- .element: class="cta-button" -->

---

## 使用 JavaScript &mdash; 建立實體

> 使用 [`document.createElement()`](https://developer.mozilla.org/docs/Web/API/Document/createElement)
> 建立實體，然後可以用 `.setAttribute()` 加以設定，最後以 `.appendChild()` 加入場景中。
> [請參考與建立實體相關的文件說明](https://aframe.io/docs/0.5.0/guides/using-javascript-and-dom-apis.html#creating-an-entity-with-createelement)。

[在 Glitch 上重混這一課的程式碼](https://glitch.com/~aframe-school-js)  <!-- .element: class="cta-button glitch" -->

1. 採用 JavaScript 的 `for` 迴圈建立 50 個 `<a-box>`，其位置與大小都隨機產生（提示：使用 `Math.random()`）

[檢視最後成果](https://aframe-school-js.glitch.me/solution3.html)  <!-- .element: class="cta-button" -->

---

## 使用 JavaScript &mdash; 處理事件

> 使用
> [`.addEventListener()`](https://developer.mozilla.org/docs/Web/API/EventTarget/addEventListener)
> 來註冊特定事件觸發時的處理函式，
> 接著再自行觸動該事件，看看處理函式是否正常運作。之後我們可以監聽事件，依據使用者輸入或其他事件來更動場景。
> [請參考 A-Frame 中使用事件及監聽式的說明文件](https://aframe.io/docs/0.5.0/guides/using-javascript-and-dom-apis.html#events-and-event-listeners)。

[在 Glitch 上重混這一課的程式碼](https://glitch.com/~aframe-school-js)  <!-- .element: class="cta-button glitch" -->

1. 監聽正方體的 `foo` 事件，並且在事件觸發時更動正方體的色彩。
2. 手動以 [`Entity.emit()`](https://aframe.io/docs/0.5.0/core/entity.html#emit-name-detail-bubbles) 觸發 `foo`，看看正方體是否正確更動色彩。

[檢視最後成果](https://aframe-school-js.glitch.me/solution4.html)  <!-- .element: class="cta-button" -->

------

## 採用視覺準心的互動方式 &mdash; 加上 cursor 實體

> 使用視覺準心的 [`cursor`
> 組件](https://aframe.io/docs/0.5.0/components/cursor.html) 來提供與實體互動的方式
> ，這種方式一般都用在智慧型手機上。 [請參考建立 360&deg; 照片集的
> 相關文件](https://aframe.io/docs/0.5.0/guides/building-with-components.html).

[在 Glitch 上重混這一課的程式碼](https://glitch.com/~aframe-school-cursor)  <!-- .element: class="cta-button glitch" -->

這一刻裡，所有事件的監聽式都已經加上去了，您只需要加上個含有 `cursor` 組件的實體，
以便透過使用者的行為觸發事件即可。需注意，這些事件並非由瀏覽器提供，而是由 A-Frame 提供。

1. 加上 [`<a-camera>`](https://aframe.io/docs/0.5.0/components/camera.html) 實體。先前的範例裡，
   A-Frame 其實提供了預設的攝影視角。
2. 加上 [`<a-cursor>`](https://aframe.io/docs/0.5.0/components/cursor.html) 實體，作為前一個攝影機
   的子實體。
3. 在桌機上，以滑鼠拖曳視角，讓準心對準面板後點擊滑鼠；在手機上，則只要移動手機注視著面板即可（此即「視覺準心」）。

<img class="stretch" data-src="media/img/gaze.gif">

[檢視最後成果](https://aframe-school-cursor.glitch.me/solution.html)  <!-- .element: class="cta-button glitch" -->

---

## 採用視覺準心的互動方式 &mdash; 處理事件

> 使用視覺準心之
> [`cursor` 組件](https://aframe.io/docs/0.5.0/components/cursor.html) 所提供的
> `click`、`mouseenter` 及 `mouseleave` 等事件來修改物件的屬性。

Glitch 上的程式已經將專案的結構都設定好了，我們接著要在 `handle-events` 組件裡（註解所提示的地方）加上 JavaScript 程式。

[在 Glitch 上重混這一課的程式碼](https://glitch.com/~aframe-school-cursor-handler-patch)  <!-- .element: class="cta-button glitch" -->

1. 將我們剛剛寫的組件 `handle-events` 加到方塊上。多種監聽、一次滿足 ;)
2. 在組件內為 `mouseenter` 事件加上監聽式，觸發時更動方塊的顏色
3. 在組件內為 `mouseleave` 事件加上監聽式，觸發時恢復方塊的顏色

<img class="stretch" data-src="media/img/gazehandler.gif">

[檢視最後成果](https://aframe-school-cursor-handler-patch.glitch.me/solution.html)  <!-- .element: class="cta-button glitch" -->

------

## 加入 3D 模型 &mdash; glTF 模型

> 3D 模型就像是在 3D 或 VR 軟體中的圖片一般，只是比較複雜一點 -- 在 3D 建模軟體（例如
> [Blender](https://www.blender.org/)） 中，你可以設定多邊形、材質、素材等等預先建立模型。
> 我們建議採用 [glTF](https://github.com/KhronosGroup/glTF)，這是針對 Web 設計的嶄新 3D 檔案格式，
> 就好像是 3D 模型版的 JPEG 檔一樣。

[在 Glitch 上重混這一課的程式碼](https://glitch.com/~aframe-school-gltf-model)  <!-- .element: class="cta-button glitch" -->

1. 為了預先載入模型，請將 `<a-asset-item id="cityModel">` 的 `src` 屬性設定為 `https://cdn.aframe.io/test-models/models/virtualcity/VC.gltf`
2. 將 `<a-gltf-model>` 的 `src` 屬性設定為 `#cityModel`，真正在場景中使用這個模型。

<img class="stretch" data-src="https://cloud.githubusercontent.com/assets/674727/24275925/63067074-0ff0-11e7-9440-7c855b9ea0fd.png">

[檢視最後成果](https://aframe-school-gltf-model.glitch.me/solution.html)  <!-- .element: class="cta-button" -->

---

## 加入 3D 模型 &mdash; glTF 模型動畫

> 模型有時會帶著動畫。方才加上的模型裡，正帶有許多船隻遊走於城市中的動畫。
> 我們可以在前一份 Glitch 上加入 `animation-mixer` 這個組件以播放其所有動畫。
> 接著我們就從上一頁的成果繼續操作。

1. 在 `<head>` 中的 A-Frame 程式之後，用個 `<script>` 引入 `animation-mixer` 組件。目前，這個組件可由 Registry 尋得，或許某天會內建於 A-Frame 之中。 `https://unpkg.com/aframe-extras.animation-mixer@3.4.0/dist/aframe-extras.animation-mixer.js`
2. 在 `<a-gltf-model>` 加上 `animation-mixer` 屬性以附加組件。預設狀態下，這樣就會將模型所自帶的所有動畫同步播放。

<img class="stretch" data-src="media/img/gltf.gif">

[檢視最後成果](https://aframe-school-gltf-model.glitch.me/solution2.html)  <!-- .element: class="cta-button" -->

---

## 加入 3D 模型 &mdash; 上傳 3D 模型

> 如果你自己建了個 3D 模型，由於當中牽扯許多相互參照的素材或檔案，想要丟上 CDN 來使用可能有點麻煩。
> 目前我們發現最簡單的方法是直接把東西丟進 GitHub repo、將該 repo 的 master 分支發布為 GitHub Pages，
> 接著使用 `rawgit.com` 來存取。或者，也可以選擇丟上 Amazon S3。日後這一頁會加上其他相關資訊。

------

## Add Tracked Controls &mdash; Add Hand Controls

> Tracked hand controls provide immersion and interactivity with hand
> controllers. In the following Glitch, we've pre-recorded hand control
> movements and button presses with [A-Frame Motion
> Capture](https://github.com/dmarcos/aframe-motion-capture-components).
> Now we just have to add the hands and handle the interaction events.

[在 Glitch 上重混這一課的程式碼](https://glitch.com/~aframe-school-hand-controls)  <!-- .element: class="cta-button glitch" -->

1. Find `<a-entity id="left">` and add the [hand-controls component](https://aframe.io/docs/0.5.0/components/hand-controls.html)
configured to the left hand (`hand-controls="left"`)
2. Find `<a-entity id="right">` and add the hand-controls component
configured to the right hand (`hand-controls="right"`)
3. View the result and see the hands moving with pre-recorded motions

<img class="stretch" data-src="media/img/trackedcontrols.gif">

[檢視最後成果](https://aframe-school-hand-controls.glitch.me/solution.html)  <!-- .element: class="cta-button" -->

---

## Add Tracked Controls &mdash; Add Interactivity

> There are many components to add interactivity to hand controls.
> [controller-cursor](https://github.com/bryik/aframe-controller-cursor-component),
> [aabb-collider +
> grab](https://github.com/aframevr/aframe/tree/master/examples/showcase/tracked-controls/components),
> [super-hands](https://github.com/wmurphyrd/aframe-super-hands-component). For
> this lesson, we'll use controller-cursor that acts as a pointing laser for
> each hand. Continue from your previous Glitch.

1. Add `controller-cursor` component to both hands
2. In the `controller-event-handler` component, change the color of the boxes
when they are hovered over with the `mouseenter` event, and restore the color
with the `mouseleave` event

<img class="stretch" data-src="media/img/trackedcontrols2.gif">

[檢視最後成果](https://aframe-school-hand-controls.glitch.me/solution2.html)  <!-- .element: class="cta-button" -->

------


<!-- Lessons end here. -->


## 恭喜！

您已經從 A-Frame 學院畢業，在此向您授與非正式的 WebVR 學位。

<img class="stretch" data-src="https://cdn.hackaday.io/images/4174761433219325627.png">

接著，您可以繼續深入[閱讀相關文件](https://aframe.io/docs/)，進一步掌握更多技巧，邁向大師之路。
