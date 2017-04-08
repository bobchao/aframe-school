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

> Fill in the `src` HTML attributes with image URLs. [Read about applying an
> image texture](https://aframe.io/docs/0.5.0/guides/#applying-an-image-texture).

[Remix Lesson on Glitch](https://glitch.com/~aframe-school-textures/)  <!-- .element: class="cta-button glitch" -->

1. Add an image texture to the ground, `<a-plane>`
2. Add image textures to `<a-box>`es
3. Add an image texture to `<a-sphere>`
4. Add an image texture to `<a-cone>`
5. Add an image texture to the background, `<a-sky>`. Find [360&deg; images from FLickr](https://www.flickr.com/groups/equirectangular/)

<img class="stretch" data-src="media/img/texture.jpg">

[View Result](https://aframe-school-textures.glitch.me/solution.html)  <!-- .element: class="cta-button" -->

------

## Open the A-Frame Inspector

> Hit **`<ctrl> + <alt> + i`** on **any** A-Frame scene to pop open a visual
> editor, just like your browser's Dev Tools!  Try the Inspector on some of the
> [homepage examples](https://aframe.io/examples/). [Read about the
> Inspector](https://aframe.io/docs/master/guides/using-the-aframe-inspector.html).

<img class="stretch" data-src="media/img/inspector.gif">

---

## Open the A-Frame Inspector &mdash; Change Component Values

> Modify an entity by modifying its components on the right-hand panel. The
> Inspector knows about all A-Frame components, including community components.
>  This example includes an external [text-geometry
> component](https://www.npmjs.com/package/aframe-text-geometry-component), which
> the Inspector can modify the values of live.

[Open Example on Glitch](https://aframe-vaporwave.glitch.me)  <!-- .element: class="cta-button glitch" -->

1. Select one of the entities with text in the example
2. Change the [`text-geometry` component's](https://www.npmjs.com/package/aframe-text-geometry-component) `value` property

<img class="stretch" data-src="media/img/inspectorchange.jpg">

---

## Open the A-Frame Inspector &mdash; Attach Components from the Registry

> Use [physics components](https://github.com/donmccurdy/aframe-physics-system)
> from the [Registry](https://aframe.io/registry/) to add gravity and collisions.
> The Registry is a curated collection of A-Frame components. And the Inspector
> is hooked up to the Registry so we can add components from the Registry in the
> entity panel.

[Open Example on Glitch](https://aframe-vaporwave.glitch.me)  <!-- .element: class="cta-button glitch" -->

1. Add the `static-body` component to ground grid
2. Add the `dynamic-body` component to the torus knot (the purple pretzel in the back)
3. Increase the Y-position of the torus knot to make it higher up
4. Exit the Inspector

<img class="stretch" data-src="media/img/inspectorregistry.gif">

------

## Compose with Entity-Component &mdash; Break Primitives Down

> Behind the easy-to-use primitive elements, A-Frame is based on an
> entity-component architecture. Decompose the primitive elements in the
> *Hello, WebVR* example to `<a-entity>`s with their fundamental components.

[Remix Lesson on Glitch](https://glitch.com/~aframe-school-ecs)  <!-- .element: class="cta-button glitch" -->

[geometry]: https://aframe.io/docs/0.5.0/components/geometry.html
[material]: https://aframe.io/docs/0.5.0/components/material.html

1. Convert `<a-box>` to `<a-entity>` with [geometry component][geometry] and [material component][material]. Configure the geometry component to be `primitive: box`
2. Convert `<a-sphere>` to `<a-entity>` with geometry component and material component. Configure the geometry component to be `primitive: sphere`
3. Convert `<a-cylinder>` to `<a-entity>` with geometry component and material component. Configure the geometry component to be `primitive: cylinder`
4. Convert `<a-plane>` to `<a-entity>` with geometry component and material component. Configure the geometry component to be `primitive: plane`
5. Convert `<a-sky>` to `<a-entity>` with geometry component and material component. Configure the geometry component to be `primitive: sphere` with a large `radius: 3000`, and configure the material component to be `shader: flat` so we don't do expensive lighting calculations when we just need a flat color

[View Result](https://aframe-school-ecs.glitch.me/solution.html)  <!-- .element: class="cta-button" -->

---

## Compose with Entity-Component &mdash; Add a Light Source Sphere

> Use the entity-component pattern to add a sphere that also acts as a point
> light source. Mix together the geometry, material, and light components to
> compose this type of object.

1. Look for `<a-entity id="lightSphere">`
2. Attach the [geometry component](https://aframe.io/docs/0.5.0/components/geometry.html) configured to use `primitive: sphere` to the entity
3. Attach the [material component](https://aframe.io/docs/0.5.0/components/material.html) configured to use `color: #FFF` and `shader: flat` to the entity
4. Attach the [light component](https://aframe.io/docs/0.5.0/components/light.html) configured to use `type: point` to the entity
5. **Extra Credit:** Add the animation component from [the Registry](https://aframe.io/registry/) via a `<script>` tag. Attach the animation configured to use `property: position` and `dir: alternate` and `loop: true` and provide a position value for `to: <POSITION>`

[Remix Lesson on Glitch](https://glitch.com/~aframe-school-ecs-light-sphere)  <!-- .element: class="cta-button glitch" -->

<img class="stretch" data-src="https://cloud.githubusercontent.com/assets/674727/24060160/2c53a604-0b0f-11e7-9386-f83a3a9b4cfc.gif">>

[View Result](https://aframe-school-ecs-light-sphere.glitch.me/solution.html)  <!-- .element class="cta-button" -->

------

## Extend with Entity-Component &mdash; From the Registry

> [The Registry](https://aframe.io/registry/) is a great place to grab cool
> components that the community has added to A-Frame. Sort of like third-party
> plugins. Find community components from the Registry, copy their JS links,
> include them via a `<script>` tag, and use them straight from HTML.

1. Include [Particle
System](https://www.npmjs.com/package/aframe-particle-system-component). Attach
`<a-entity>`s with `particle-system` components configured to `preset: default`
and `preset: snow`. Open the Inspector to play with the values!
2. Include [Animation](https://www.npmjs.com/package/aframe-animation-component). Attach
animation to the sphere to throb its scale by configuring `animation` component
with `property: scale`, `loop: true`, and `to: 1.1 1.1 1.1`
3. Include [Outline Effect](https://www.npmjs.com/package/aframe-outline-effect). Drop in the
`<script>` and attach the `outline` component to the scene

[Remix Lesson on Glitch](https://glitch.com/~aframe-school-registry)  <!-- .element: class="cta-button glitch" -->

<img class="stretch" data-src="media/img/registryexample.gif">

[View Result](https://aframe-school-registry.glitch.me/solution.html)  <!-- .element class="cta-button" -->

------

## Use JavaScript

> Use JavaScript and DOM APIs to programmatically modify the scene and its
> entities. A-Frame is not just HTML; A-Frame provides access to JavaScript,
> DOM APIs, and three.js underneath for full control.  [Read about *Using
> JavaScript and DOM APIs* with
> A-Frame](https://aframe.io/docs/0.5.0/guides/using-javascript-and-dom-apis.html).

[Remix Lesson on Glitch](https://glitch.com/~aframe-school-js)  <!-- .element: class="cta-button glitch" -->

<img class="stretch" data-src="media/img/js.jpg">

To see JavaScript logs, we can open the browser's development console by
right-clicking the page, clicking *Inspect* or *Inspect Element*, and then
clicking the *Console* tab. When viewing solutions, we can see the results
through the browser console.

---

## Use JavaScript &mdash; Getting Entities

> Use
> [`document.querySelector()`](https://developer.mozilla.org/docs/Web/API/Document/querySelector)
> and
> [`document.querySelectorAll()`](https://developer.mozilla.org/docs/Web/API/Document/querySelectorAll)
> to get a reference to the scene and its entities.  [Read about querying for
> entities](https://aframe.io/docs/0.5.0/guides/using-javascript-and-dom-apis.html#getting-entities-by-querying-and-traversing).

[Remix Lesson on Glitch](https://glitch.com/~aframe-school-js)  <!-- .element: class="cta-button glitch" -->

1. Get a reference to the `<a-scene>` element using `var sceneEl = document.querySelector('a-scene');`
2. Get a reference to all `<a-entity>` elements using `sceneEl.querySelectorAll('a-entity');`
3. Get a reference to the box entity using `sceneEl.querySelector('#box');`
4. Get a reference to the sphere and cylinder entities in one `.querySelectorAll()` call by using multi-element selector
. Get a reference to the sphere and cylinder entities in one `.querySelectorAll()` call by adding and selecting HTML classes

[View Result](https://aframe-school-js.glitch.me/solution.html)  <!-- .element: class="cta-button" -->

---

## Use JavaScript &mdash; Modifying Entities

> Use
> [`Entity.setAttribute()`](https://aframe.io/docs/0.5.0/core/entity.html#setattribute-attr-value-componentattrvalue)
> to modify entities after retrieving them from the previous exercise. [Read
> about modifying
> entities](https://aframe.io/docs/0.5.0/guides/using-javascript-and-dom-apis.html#modifying-an-entity).

[Remix Lesson on Glitch](https://glitch.com/~aframe-school-js)  <!-- .element: class="cta-button glitch" -->

1. Change the box entity's `rotation` component
2. Change the cylinder entity's `geometry` component's `height` property
3. Change the sphere entity's `material` component's `metalness` property

[View Result](https://aframe-school-js.glitch.me/solution2.html)  <!-- .element: class="cta-button" -->

---

## Use JavaScript &mdash; Creating Entities

> Use [`document.createElement()`](https://developer.mozilla.org/docs/Web/API/Document/createElement)
> to create entities, `.setAttribute()` to configure them, and `.appendChild()`
> to add them to the scene.  [Read about creating
> entities](https://aframe.io/docs/0.5.0/guides/using-javascript-and-dom-apis.html#creating-an-entity-with-createelement).

[Remix Lesson on Glitch](https://glitch.com/~aframe-school-js)  <!-- .element: class="cta-button glitch" -->

1. In a JavaScript `for` loop, create and add 50 `<a-box>` elements with
random positions and scales (use `Math.random()`)

[View Result](https://aframe-school-js.glitch.me/solution3.html)  <!-- .element: class="cta-button" -->

---

## Use JavaScript &mdash; Handling Events

> Use
> [`.addEventListener()`](https://developer.mozilla.org/docs/Web/API/EventTarget/addEventListener)
> to register a handler function that will be called when an event is emitted.
> Then manually emit that event to see that handler function execute. Later we
> can use event listeners to change the scene based on user input or other
> events. [Read about events and event listeners with
> A-Frame](https://aframe.io/docs/0.5.0/guides/using-javascript-and-dom-apis.html#events-and-event-listeners).

[Remix Lesson on Glitch](https://glitch.com/~aframe-school-js)  <!-- .element: class="cta-button glitch" -->

1. Register an event listener on the box to listen to the `foo` event. In the
   handler function, change the box's color
2. Emit the `foo` event with
[`Entity.emit()`](https://aframe.io/docs/0.5.0/core/entity.html#emit-name-detail-bubbles)
and see the box change its color

[View Result](https://aframe-school-js.glitch.me/solution4.html)  <!-- .element: class="cta-button" -->

------

## Add Gaze-Based Cursor Interactions &mdash; Add Cursor Entity

> Use the gaze-based [`cursor`
> component](https://aframe.io/docs/0.5.0/components/cursor.html) to provide
> the ability to interact with entities (primarily for smartphones).  [Read
> about building a 360&deg; image
> gallery](https://aframe.io/docs/0.5.0/guides/building-with-components.html).

[Remix Lesson on Glitch](https://glitch.com/~aframe-school-cursor)  <!-- .element: class="cta-button glitch" -->

This lesson has all the event listeners hooked up already. We just need to add
an entity with the `cursor` component which will provide those events based on
user input.  Note these events are not provided by the browser, but through
A-Frame.

1. Add [`<a-camera>`](https://aframe.io/docs/0.5.0/components/camera.html) entity.
   Previously A-Frame was providing a default camera
2. Add [`<a-cursor>`](https://aframe.io/docs/0.5.0/components/cursor.html) entity
   as a child underneath the camera entity
3. Drag the camera around the click on the panels on desktop. On smartphones,
   stare at the panels to trigger clicks (i.e., gaze-based)

<img class="stretch" data-src="media/img/gaze.gif">

[View Result](https://glitch.com/~aframe-school-cursor)  <!-- .element: class="cta-button glitch" -->

---

## Add Gaze-Based Cursor Interactions &mdash; Handle Events

> Use the `click`, `mouseenter`, `mouseleave` events provided by the gaze-based
> [`cursor` component](https://aframe.io/docs/0.5.0/components/cursor.html) to
> change the properties of an object.

The Glitch code will have the project structure set up. We can add JavaScript
code inside the `handle-events` component, marked by the code comments.

[Remix Lesson on Glitch](https://glitch.com/~aframe-school-cursor-handler)  <!-- .element: class="cta-button glitch" -->

1. Attach our `controller-event-handler` to the cubes. We can attach to all of them at once through the mixin
2. Add an event listener to change the box's color on `mouseenter` event
3. Add an event listener to restore the box's color on `mouseleave` event

<img class="stretch" data-src="media/img/gazehandler.gif">

[View Result](https://aframe-school-cursor-handler.glitch.me/solution.html)  <!-- .element: class="cta-button glitch" -->

------

## Add 3D Models &mdash; glTF Model

> 3D models are like the images of 3D and VR applications, although a bit
> heavier. A 3D model is created beforehand in a 3D modeling program such as
> [Blender](https://www.blender.org/) and consists of vertices, textures,
> materials. We recommend using [glTF](https://github.com/KhronosGroup/glTF), a
> relatively new 3D file format standard tailored for the Web. glTF is like the
> JPG of 3D models.

[Remix Lesson on Glitch](https://glitch.com/~aframe-school-gltf-model)  <!-- .element: class="cta-button glitch" -->

1. Add the `https://cdn.aframe.io/test-models/models/virtualcity/VC.gltf` to
the `<a-asset-item id="model">`'s `src` attribute to preload the model
2. Add `#model` to the `<a-gltf-model>`'s `src` attribute to set and add the model

<img class="stretch" data-src="https://cloud.githubusercontent.com/assets/674727/24275925/63067074-0ff0-11e7-9440-7c855b9ea0fd.png">

[View Result](https://aframe-school-gltf-model.glitch.me/solution.html)  <!-- .element: class="cta-button" -->

---

## Add 3D Models &mdash; glTF Model Animations

> Models can come with animations. The model provided above has many animations
> of ships zooming across the city. In the previous Glitch, we've provided a simple
> `play-all-model-animations` component that we can attach to our model to play
> its animations. Continue working from your current Glitch.

1. Include the `animation-mixer` component via a `<script>` in the
`<head>` after the A-Frame script. This component is currently in the Registry,
and may one day be included with A-Frame. `https://unpkg.com/aframe-extras.animation-mixer@3.4.0/dist/aframe-extras.animation-mixer.js`
2. Attach the `animation-mixer` component to the `<a-gltf-model>` by
setting it via an HTML attribute `animation-mixer`. By default, this will play all
the animations of the model at once.

<img class="stretch" data-src="media/img/gltf.gif">

[View Result](https://aframe-school-gltf-model.glitch.me/solution2.html)  <!-- .element: class="cta-button" -->

---

## Add 3D Models &mdash; Uploading 3D Models

> If you have a model of your own, it can be tricky to upload it to a CDN since
> it consists of multiple files that reference each other. So far the easiest
> way we've found is to dump them into a GitHub repo, publish the repo's master
> branch to GitHub Pages, and use `rawgit.com` to serve them. Alternatively,
> set up Amazon S3. More to come.

------

## Add Tracked Controls &mdash; Add Hand Controls

> Tracked hand controls provide immersion and interactivity with hand
> controllers. In the following Glitch, we've pre-recorded hand control
> movements and button presses with [A-Frame Motion
> Capture](https://github.com/dmarcos/aframe-motion-capture-components).
> Now we just have to add the hands and handle the interaction events.

[Remix Lesson on Glitch](https://glitch.com/~aframe-school-hand-controls)  <!-- .element: class="cta-button glitch" -->

1. Find `<a-entity id="left">` and add the [hand-controls component](https://aframe.io/docs/0.5.0/components/hand-controls.html)
configured to the left hand (`hand-controls="left"`)
2. Find `<a-entity id="right">` and add the hand-controls component
configured to the right hand (`hand-controls="right"`)
3. View the result and see the hands moving with pre-recorded motions

<img class="stretch" data-src="media/img/trackedcontrols.gif">

[View Result](https://aframe-school-hand-controls.glitch.me/solution.html)  <!-- .element: class="cta-button" -->

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

[View Result](https://aframe-school-hand-controls.glitch.me/solution2.html)  <!-- .element: class="cta-button" -->

------


<!-- Lessons end here. -->


## Congratulations!

You've graduated from the A-Frame School and now have a virtual uncertified
degree in WebVR.

<img class="stretch" data-src="https://cdn.hackaday.io/images/4174761433219325627.png">

Head to [the documentation](https://aframe.io/docs/) for more guides to become
a master.
