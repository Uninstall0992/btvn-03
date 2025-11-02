---
# try also 'default' to start simple
theme: apple-basic
# random image from a curated Unsplash collection by Anthony
# like them? see https://unsplash.com/collections/94734566/slidev
background: https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Finterlink-static0.tsbohemia.cz%2Fwacom-cintiq-27qhd-touch-image3-big_ies2152048.jpg&f=1&nofb=1&ipt=23f71266e63d3c0766c635e54b78011118da895ab3b93be70545b9f39b0323b9
# some information about your slides (markdown enabled)
title: Bản vẽ - bút vẽ
# apply UnoCSS classes to the current slide
class: text-center
# https://sli.dev/features/drawing
drawings:
  persist: false
# slide transition: https://sli.dev/guide/animations.html#slide-transitions
transition: slide-left
# enable MDC Syntax: https://sli.dev/features/mdc
mdc: true
# duration of the presentation
preload: true
---

# Bản vẽ - bút vẽ

Công cụ tối thượng của những họa sĩ kĩ thuật số.

<div @click="$slidev.nav.next" class="mt-12 py-1" hover:bg="white op-10">
  Nhấn Space để di chuyển đến trang tiếp theo. <carbon:arrow-right />
</div>

<!--
The last comment block of each slide will be treated as slide notes. It will be visible and editable in Presenter Mode along with the slide. [Read more in the docs](https://sli.dev/guide/syntax.html#notes)
-->

---
transition: slide-up
level: 2
---

# Di chuyển
## Phím tắt
|                                                     |                             |
| --------------------------------------------------- | --------------------------- |
| <kbd>right</kbd> / <kbd>space</kbd>                 | hoạt động hoặc slide tiếp theo     |
| <kbd>left</kbd>  / <kbd>shift</kbd><kbd>space</kbd> | hoạt động hoặc slide trước |
| <kbd>up</kbd>                                       | slide trước              |
| <kbd>down</kbd>                                     | slide tiếp theo                  |
| <kbd>enter</kbd>                                    | tự động chạy                |
| <kbd>esc</kbd>                                      | tắt tự động chạy            |
<!-- https://sli.dev/guide/animations.html#click-animation -->

---
layout: two-cols
layoutClass: gap-16
---

# Mục lục

::right::

<Toc text-sm minDepth="1" maxDepth="2" />

---
transiton: fade
layout: fact
---

# Khái niệm
Bảng vẽ kỹ thuật số là một thiết bị đầu vào cho phép người dùng vẽ tay, hình ảnh động và đồ họa, với một thiết bị vẽ giống như bút gọi là bút vẽ, tương tự như cách một người vẽ hình ảnh bằng bút chì và giấy. [Nguồn](https://www.webopedia.com/definitions/digitizing-tablet/)

---
image: 
---

# Đặc điểm

## Bảng vẽ

<span>Bảng vẽ kỹ thuật có thể là một trong ba loại sau đây, mỗi loại mang theo những đặc điểm riêng biệt cuả nó</span>

<div mt-6 />

<div grid grid-cols-3 gap-3 h-75>

<v-clicks>

<div border="2 solid white/5" rounded-lg overflow-hidden bg="white/5" backdrop-blur-sm h-full>
  <div flex items-center bg="white/10" backdrop-blur px-3 py-2 rounded-md>
    <div i-carbon:draw text-amber-300 text-sm mr-2 />
    <div font-semibold>
      Bảng vẽ đơn giản
    </div>
  </div>
  <div px-4 py-3>
    <div flex flex-col gap-3>
      <div>
        <div text-sm font-medium>Tấm vẽ đơn giản</div>
        <div text-xs opacity-70>Phải kết nối vào máy tính để sử dụng với bút</div>
      </div>
      <div>
        <div text-sm font-medium>Đòi hỏi kỹ năng</div>
        <div text-xs opacity-70>Người dùng vừa pahỉ nhìn màn hình máy tính vừa phải chuyển động tay</div>
      </div>
      <div>
        <div text-sm font-medium>Giá thành thấp</div>
        <div text-xs opacity-70>Giao động phải chăng kể cả với bảng lớn</div>
      </div>
      <div>
        <div text-sm font-medium>Chống gù</div>
        <div text-xs opacity-70>Người dùng không cần cúi người xuống khi dùng như các loại có màn hình </div>
      </div>
    </div>
  </div>
</div>

<div border="2 solid white/5" rounded-lg overflow-hidden bg="white/5" backdrop-blur-sm h-full>
  <div flex items-center bg="white/10" backdrop-blur px-3 py-2 rounded-md>
    <div i-carbon:tablet-landscape text-blue-300 text-sm mr-2 />
    <div font-semibold>
      Bảng vẽ màn hình
    </div>
  </div>
  <div px-4 py-3>
    <div flex flex-col gap-3>
      <div>
        <div text-sm font-medium>Gắn màn hình</div>
        <div text-xs opacity-70>Người dùng vẽ trực tiếp lên bảng vẽ</div>
      </div>
      <div>
        <div text-sm font-medium>Giá thành cao</div>
        <div text-xs opacity-70>Có thể đắt bằng các máy tính, laptop tầm trung đặc biệt là với những màn hình lớn</div>
      </div>
    </div>
  </div>
</div>

<div border="2 solid white/5" rounded-lg overflow-hidden bg="white/5" backdrop-blur-sm h-full>
  <div flex items-center bg="white/10" backdrop-blur px-3 py-2 rounded-md>
    <div i-carbon:screen text-green-300 text-sm mr-2 />
    <div font-semibold>
      Bảng vẽ máy tính
    </div>
  </div>
  <div px-4 py-3>
    <div flex flex-col gap-3>
      <div>
        <div text-sm font-medium>Tích hợp máy tính</div>
        <div text-xs opacity-70>Không cần máy tính để chạy phần mềm vẽ</div>
      </div>
      <div>
        <div text-sm font-medium>Giá thành rất cao</div>
        <div text-xs opacity-70>Có thể đắt bằng các máy tính, laptop cao cấp</div>
      </div>
    </div>
  </div>
</div>

</v-clicks>

</div>

<div v-click mt-6 flex justify-center>
  <div
    border="2 solid white/5" bg="white/5" backdrop-blur-sm
    rounded-lg px-6 py-3 flex items-center gap-3
  >
    <div i-carbon:idea text-yellow-300 text-2xl />
    <span text-lg>Có mọi bảng vẽ kỹ thuật cho mọi kinh phí, kinh nghiệm và nhu cầu sử dụng</span>
  </div>
</div>

---
layout: 3-images
imageLeft: 'https://www.zdnet.com/a/img/resize/a0b30b508195956bd9fcd92d5ff1572eaeb78cd4/2023/02/16/35775989-197a-43ce-8c97-13936dde5f4f/pxl-20230216-173948408.jpg?auto=webp&fit=crop&height=900&width=1200'
imageTopRight: 'https://astropad.com/wp-content/uploads/2024/01/Wacom-Cintiq-16-.webp'
imageBottomRight: 'https://store-img.huion.com.cn/3/a6c/standalone-tablet-mobile.webp'
---

---

## Bút cảm ứng

<span>Bút cảm ứng hoạt động theo hai nguyên lý căn bản: Điện dung và cộng hưởng điện từ. Hai nguyên lý này quyết định khả năng chuyển động của bút được nhận diện.</span>

<div mt-6 grid grid-cols-2 gap-6>
  <div
    v-click
    border="2 solid red-800" bg="red-800/20"
    rounded-lg overflow-hidden
  >
    <div bg="red-800/40" px-4 py-2 flex items-center>
      <div i-carbon:warning-alt text-red-300 text-xl mr-2 />
      <span font-bold>Điện dung</span>
    </div>
    <div px-4 py-3 flex flex-col gap-2>
      <div flex items-center gap-2 py-1>
        <div i-carbon:development text-amber-300 text-xl />
        <div>
          <div font-bold>Development</div>
          <div text-sm opacity-80>Preparing new model training datasets</div>
        </div>
      </div>
      <div flex items-center gap-2 py-1>
        <div i-carbon:machine-learning-model text-amber-300 text-xl />
        <div>
          <div font-bold>Nhận dạng</div>
          <div text-sm opacity-80>Fine-tuning load with transformers lib</div>
        </div>
      </div>
      <div flex items-center gap-2 py-1>
        <div i-carbon:user-certification text-amber-300 text-xl />
        <div>
          <div font-bold>Chuyên dụng</div>
          <div text-sm opacity-80>Chỉ hoạt động với thiết bị được hỗ trợ</div>
        </div>
      </div>
    </div>
  </div>

  <div
    v-click
    border="2 solid green-800" bg="green-800/20"
    rounded-lg overflow-hidden
  >
    <div bg="green-800/40" px-4 py-2 flex items-center>
      <div i-carbon:cloud-service-management text-green-300 text-xl mr-2 />
      <span font-bold>Cộng hưởng điện từ</span>
    </div>
    <div px-4 py-3 flex flex-col gap-2 h-full>
      <div bg="green-900/30" rounded-lg p-3 flex flex-col gap-2>
        <div font-bold text-sm>Single Environment, Multiple Contexts</div>
        <div flex items-center gap-2>
          <div i-carbon:checkmark-outline text-green-400 />
          <span text-sm>Define once, use everywhere</span>
        </div>
        <div flex items-center gap-2>
          <div i-carbon:checkmark-outline text-green-400 />
          <span text-sm>Tracked dependencies with lockfiles</span>
        </div>
        <div flex items-center gap-2>
          <div i-carbon:checkmark-outline text-green-400 />
          <span text-sm>Automatic dependency resolution</span>
        </div>
      </div>
    </div>
  </div>
</div>

---
level: 2
---

# Shiki Magic Move

Powered by [shiki-magic-move](https://shiki-magic-move.netlify.app/), Slidev supports animations across multiple code snippets.

Add multiple code blocks and wrap them with <code>````md magic-move</code> (four backticks) to enable the magic move. For example:

````md magic-move {lines: true}
```ts {*|2|*}
// step 1
const author = reactive({
  name: 'John Doe',
  books: [
    'Vue 2 - Advanced Guide',
    'Vue 3 - Basic Guide',
    'Vue 4 - The Mystery'
  ]
})
```

```ts {*|1-2|3-4|3-4,8}
// step 2
export default {
  data() {
    return {
      author: {
        name: 'John Doe',
        books: [
          'Vue 2 - Advanced Guide',
          'Vue 3 - Basic Guide',
          'Vue 4 - The Mystery'
        ]
      }
    }
  }
}
```

```ts
// step 3
export default {
  data: () => ({
    author: {
      name: 'John Doe',
      books: [
        'Vue 2 - Advanced Guide',
        'Vue 3 - Basic Guide',
        'Vue 4 - The Mystery'
      ]
    }
  })
}
```

Non-code blocks are ignored.

```vue
<!-- step 4 -->
<script setup>
const author = {
  name: 'John Doe',
  books: [
    'Vue 2 - Advanced Guide',
    'Vue 3 - Basic Guide',
    'Vue 4 - The Mystery'
  ]
}
</script>
```
````

---

# Components

<div grid="~ cols-2 gap-4">
<div>

You can use Vue components directly inside your slides.

We have provided a few built-in components like `<Tweet/>` and `<Youtube/>` that you can use directly. And adding your custom components is also super easy.

```html
<Counter :count="10" />
```

<!-- ./components/Counter.vue -->
<Counter :count="10" m="t-4" />

Check out [the guides](https://sli.dev/builtin/components.html) for more.

</div>
<div>

```html
<Tweet id="1390115482657726468" />
```

<Tweet id="1390115482657726468" scale="0.65" />

</div>
</div>

<!--
Presenter note with **bold**, *italic*, and ~~striked~~ text.

Also, HTML elements are valid:
<div class="flex w-full">
  <span style="flex-grow: 1;">Left content</span>
  <span>Right content</span>
</div>
-->

---
class: px-20
---

# Themes

Slidev comes with powerful theming support. Themes can provide styles, layouts, components, or even configurations for tools. Switching between themes by just **one edit** in your frontmatter:

<div grid="~ cols-2 gap-2" m="t-2">

```yaml
---
theme: default
---
```

```yaml
---
theme: seriph
---
```

<img border="rounded" src="https://github.com/slidevjs/themes/blob/main/screenshots/theme-default/01.png?raw=true" alt="">

<img border="rounded" src="https://github.com/slidevjs/themes/blob/main/screenshots/theme-seriph/01.png?raw=true" alt="">

</div>

Read more about [How to use a theme](https://sli.dev/guide/theme-addon#use-theme) and
check out the [Awesome Themes Gallery](https://sli.dev/resources/theme-gallery).

---

# Clicks Animations

You can add `v-click` to elements to add a click animation.

<div v-click>

This shows up when you click the slide:

```html
<div v-click>This shows up when you click the slide.</div>
```

</div>

<br>

<v-click>

The <span v-mark.red="3"><code>v-mark</code> directive</span>
also allows you to add
<span v-mark.circle.orange="4">inline marks</span>
, powered by [Rough Notation](https://roughnotation.com/):

```html
<span v-mark.underline.orange>inline markers</span>
```

</v-click>

<div mt-20 v-click>

[Learn more](https://sli.dev/guide/animations#click-animation)

</div>

---

# Motions

Motion animations are powered by [@vueuse/motion](https://motion.vueuse.org/), triggered by `v-motion` directive.

```html
<div
  v-motion
  :initial="{ x: -80 }"
  :enter="{ x: 0 }"
  :click-3="{ x: 80 }"
  :leave="{ x: 1000 }"
>
  Slidev
</div>
```

<div class="w-60 relative">
  <div class="relative w-40 h-40">
    <img
      v-motion
      :initial="{ x: 800, y: -100, scale: 1.5, rotate: -50 }"
      :enter="final"
      class="absolute inset-0"
      src="https://sli.dev/logo-square.png"
      alt=""
    />
    <img
      v-motion
      :initial="{ y: 500, x: -100, scale: 2 }"
      :enter="final"
      class="absolute inset-0"
      src="https://sli.dev/logo-circle.png"
      alt=""
    />
    <img
      v-motion
      :initial="{ x: 600, y: 400, scale: 2, rotate: 100 }"
      :enter="final"
      class="absolute inset-0"
      src="https://sli.dev/logo-triangle.png"
      alt=""
    />
  </div>

  <div
    class="text-5xl absolute top-14 left-40 text-[#2B90B6] -z-1"
    v-motion
    :initial="{ x: -80, opacity: 0}"
    :enter="{ x: 0, opacity: 1, transition: { delay: 2000, duration: 1000 } }">
    Slidev
  </div>
</div>

<!-- vue script setup scripts can be directly used in markdown, and will only affects current page -->
<script setup lang="ts">
const final = {
  x: 0,
  y: 0,
  rotate: 0,
  scale: 1,
  transition: {
    type: 'spring',
    damping: 10,
    stiffness: 20,
    mass: 2
  }
}
</script>

<div
  v-motion
  :initial="{ x:35, y: 30, opacity: 0}"
  :enter="{ y: 0, opacity: 1, transition: { delay: 3500 } }">

[Learn more](https://sli.dev/guide/animations.html#motion)

</div>

---

# LaTeX

LaTeX is supported out-of-box. Powered by [KaTeX](https://katex.org/).

<div h-3 />

Inline $\sqrt{3x-1}+(1+x)^2$

Block
$$ {1|3|all}
\begin{aligned}
\nabla \cdot \vec{E} &= \frac{\rho}{\varepsilon_0} \\
\nabla \cdot \vec{B} &= 0 \\
\nabla \times \vec{E} &= -\frac{\partial\vec{B}}{\partial t} \\
\nabla \times \vec{B} &= \mu_0\vec{J} + \mu_0\varepsilon_0\frac{\partial\vec{E}}{\partial t}
\end{aligned}
$$

[Learn more](https://sli.dev/features/latex)

---

# Diagrams

You can create diagrams / graphs from textual descriptions, directly in your Markdown.

<div class="grid grid-cols-4 gap-5 pt-4 -mb-6">

```mermaid {scale: 0.5, alt: 'A simple sequence diagram'}
sequenceDiagram
    Alice->John: Hello John, how are you?
    Note over Alice,John: A typical interaction
```

```mermaid {theme: 'neutral', scale: 0.8}
graph TD
B[Text] --> C{Decision}
C -->|One| D[Result 1]
C -->|Two| E[Result 2]
```

```mermaid
mindmap
  root((mindmap))
    Origins
      Long history
      ::icon(fa fa-book)
      Popularisation
        British popular psychology author Tony Buzan
    Research
      On effectiveness<br/>and features
      On Automatic creation
        Uses
            Creative techniques
            Strategic planning
            Argument mapping
    Tools
      Pen and paper
      Mermaid
```

```plantuml {scale: 0.7}
@startuml

package "Some Group" {
  HTTP - [First Component]
  [Another Component]
}

node "Other Groups" {
  FTP - [Second Component]
  [First Component] --> FTP
}

cloud {
  [Example 1]
}

database "MySql" {
  folder "This is my folder" {
    [Folder 3]
  }
  frame "Foo" {
    [Frame 4]
  }
}

[Another Component] --> [Example 1]
[Example 1] --> [Folder 3]
[Folder 3] --> [Frame 4]

@enduml
```

</div>

Learn more: [Mermaid Diagrams](https://sli.dev/features/mermaid) and [PlantUML Diagrams](https://sli.dev/features/plantuml)

---
foo: bar
dragPos:
  square: 691,32,167,_,-16
---

# Draggable Elements

Double-click on the draggable elements to edit their positions.

<br>

###### Directive Usage

```md
<img v-drag="'square'" src="https://sli.dev/logo.png">
```

<br>

###### Component Usage

```md
<v-drag text-3xl>
  <div class="i-carbon:arrow-up" />
  Use the `v-drag` component to have a draggable container!
</v-drag>
```

<v-drag pos="663,206,261,_,-15">
  <div text-center text-3xl border border-main rounded>
    Double-click me!
  </div>
</v-drag>

<img v-drag="'square'" src="https://sli.dev/logo.png">

###### Draggable Arrow

```md
<v-drag-arrow two-way />
```

<v-drag-arrow pos="67,452,253,46" two-way op70 />

---
src: ./pages/imported-slides.md
hide: false
---

---

# Monaco Editor

Slidev provides built-in Monaco Editor support.

Add `{monaco}` to the code block to turn it into an editor:

```ts {monaco}
import { ref } from 'vue'
import { emptyArray } from './external'

const arr = ref(emptyArray(10))
```

Use `{monaco-run}` to create an editor that can execute the code directly in the slide:

```ts {monaco-run}
import { version } from 'vue'
import { emptyArray, sayHello } from './external'

sayHello()
console.log(`vue ${version}`)
console.log(emptyArray<number>(10).reduce(fib => [...fib, fib.at(-1)! + fib.at(-2)!], [1, 1]))
```

---
layout: center
class: text-center
---

# Learn More

[Documentation](https://sli.dev) · [GitHub](https://github.com/slidevjs/slidev) · [Showcases](https://sli.dev/resources/showcases)

<PoweredBySlidev mt-10 />
