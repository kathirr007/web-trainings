--- Introduction
layout: cover
title: Vue.js Training
titleTemplate: '%s | Capgemini'
favicon: "/images/capgemini-logo-icon.png"
highlighter: shiki
css: unocss
colorSchema: dark
transition: fade-out
mdc: true
download: true
export:
  format: pdf
  timeout: 100000
  dark: false
  withClicks: false
  withToc: false
---

<h1 flex="~ col">
<div>Vue.js</div>
<div><b font-bold>The Progressive Framework</b></div>
</h1>

<div uppercase text-sm tracking-widest>
Kathiravan K
</div>

<div abs-br m-3 flex="~ col" text-sm text-right>
  <img src="/images/capgemini-logo.png" />
</div>

---
layout: intro
glowX: 10
glowY: 90
style: 'padding-left: 8rem;'
---

# Kathiravan K

<div class="w-60% opacity-80">
Senior Software Engineer
With 11+ Years of experience in Web and UI Development
And 5+ Years of experience in Vue.js.
</div>

<div my-10 w-min flex="~ gap-1" items-center justify-center>
  <div i-ri-user-3-line op50 ma text-xl/>
  <div><a href="https://kathirr007.vercel.app/" target="_blank" class="border-none! font-300">kathirr007</a></div>
  <div i-ri-github-line op50 ma text-xl ml4/>
  <div><a href="https://github.com/kathirr007" target="_blank" class="border-none! font-300">kathirr007</a></div>
  <div i-ri-twitter-line op50 ma text-xl ml4/>
  <div><a href="https://x.com/kathirr_007" target="_blank" class="border-none! font-300">kathirr_007</a></div>
</div>

<img src="https://gravatar.com/avatar/a5630d956d792e81b5f9a60f7d65e1d0?size=320" rounded-full w-35 abs-tr mt-32 mr-40/>

<div flex="~ gap2">

</div>

---
layout: full
glowX: 0
glowY: 90
---

<h2 mb-4>Day 1 - Agenda</h2>
<ul>
  <li><a href="/4">Introduction</a></li>
  <li><a href="/11">Quick Start</a></li>
</ul>

<!-- <SharedCopyright /> -->

---
layout: full
glowX: 90
glowY: 0
---

<h2 mb-4>Introduction</h2>
<h3 mb-2>What is Vue?</h3>
<p text-sm leading-tight>
  Vue (pronounced /vjuː/, like view) is a JavaScript framework for building user interfaces. It builds on top of standard HTML, CSS, and JavaScript and provides a declarative, component-based programming model that helps you efficiently develop user interfaces of any complexity.
</p>

<div text-xs leading-tight max-h-300px overflow-auto my-4>

  <p text-sm mt-3>Here is a minimal example:</p>

  ```js {*}{lines:true}
  import { createApp } from 'vue'
  createApp({
    data() {
      return {
        count: 0
      }
    }
  }).mount('#app')
  ```
  ```html
  <div id="app">
    <button @click="count++">
      Count is: {{ count }}
    </button>
  </div>
  ```
  <p text-sm class="!mb-0">Result:</p>

  <SimpleCounter />

  <div my-3>
    <div class="text-sm mb-2">
      The above example demonstrates the two core features of Vue:
    </div>
    <ul>
      <li>Declarative Rendering: Vue extends standard HTML with a template syntax that allows us to declaratively describe HTML output based on JavaScript state.</li>
      <li>Reactivity: Vue automatically tracks JavaScript state changes and efficiently updates the DOM when changes happen.</li>
    </ul>
  </div>
</div>

<!-- <SharedCopyright /> -->

<style scoped>
p {
  margin: 0;
}
</style>
---
layout: full
glowX: 0
glowY: 90
---

<h2 mb-4>Introduction</h2>
<h3 mb-2>The Progressive Framework</h3>
<div class="text-sm leading-normal">Vue is a framework and ecosystem that covers most of the common features needed in frontend development. But the web is extremely diverse - the things we build on the web may vary drastically in form and scale. With that in mind, Vue is designed to be flexible and incrementally adoptable. Depending on your use case, Vue can be used in different ways:</div>

<div text-sm leading-normal max-h-300px overflow-auto my-4 flex="~ col gap-2">
  <ul class="">
    <li v-click>Enhancing static HTML without a build step</li>
    <li v-click>Embedding as Web Components on any page</li>
    <li v-click>Single-Page Application (SPA)</li>
    <li v-click>Fullstack / Server-Side Rendering (SSR)</li>
    <li v-click>Jamstack / Static Site Generation (SSG)</li>
    <li v-click>Targeting desktop, mobile, WebGL, and even the terminal</li>
  </ul>
  <div v-click>If you are an experienced developer interested in how to best integrate Vue into your stack, or you are curious about what these terms mean, we discuss them in more detail in <a target="_blank" text-emerald-400 href="https://vuejs.org/guide/extras/ways-of-using-vue.html">Ways of Using Vue</a>.</div>

  <div v-click>Despite the flexibility, the core knowledge about how Vue works is shared across all these use cases. Even if you are just a beginner now, the knowledge gained along the way will stay useful as you grow to tackle more ambitious goals in the future. If you are a veteran, you can pick the optimal way to leverage Vue based on the problems you are trying to solve, while retaining the same productivity. This is why we call Vue "The Progressive Framework": it's a framework that can grow with you and adapt to your needs.</div>
</div>

<!-- <SharedCopyright /> -->

<style scoped>
p {
  margin: 0;
}
</style>
---
layout: full
glowX: 0
glowY: 90
---

<h2 mb-4>Introduction</h2>
<h3 mb-2>Single File Component</h3>
<div class="text-sm leading-normal">
  In most build-tool-enabled Vue projects, we author Vue components using an HTML-like file format called Single-File Component (also known as *.vue files, abbreviated as SFC). A Vue SFC, as the name suggests, encapsulates the component's logic (JavaScript), template (HTML), and styles (CSS) in a single file. Here's the previous example, written in SFC format:
</div>

<div text-sm leading-normal max-h-300px overflow-auto my-4 flex="~ col gap-2">
<div v-click>
<h5>SFC Example for Options API</h5>

<<< @/snippets/SFC-OptionsAPI.vue vue

</div>
</div>
---
layout: full
glowX: 0
glowY: 90
---

<h2 mb-4>Introduction</h2>
<h3 mb-2>Single File Component Cont<span tracking-wider> ...</span></h3>

<div text-sm leading-normal max-h-300px overflow-auto my-4 flex="~ col gap-2">
<div v-click>
<h5>SFC Example for Composition API</h5>

<<< @/snippets/SFC-CompositionAPI.vue vue

</div>
</div>

---
layout: full
glowX: 100
glowY: 50
---

<h2 mb-4>Introduction</h2>
<h3 mb-2>API Styles</h3>
<div class="text-sm leading-normal">
  Vue components can be authored in two different API styles: <strong text-emerald-400>Options API</strong> and <strong text-emerald-400>Composition API</strong>.
</div>

<div text-sm leading-normal max-h-300px overflow-auto my-4 flex="~ col gap-2">
<div v-click>
<h5 text-lg mb-2>Options API</h5>
<div text-sm leading-normal>
  With Options API, we define a component's logic using an object of options such as <code text-emerald-400>data</code>, <code text-emerald-400>methods</code>, and <code text-emerald-400>mounted</code>. Properties defined by options are exposed on this inside functions, which points to the component instance:
</div>
<<< @/snippets/APIStyle-OptionsAPI.vue vue
</div>
</div>
---
layout: full
glowX: 100
glowY: 50
---

<h2 mb-4>Introduction</h2>
<h3 mb-2>API Styles Cont <span tracking-wider>...</span></h3>

<div text-sm leading-normal max-h-300px overflow-auto my-4 flex="~ col gap-2">
<div flex="~ col gap-2" v-click>
<h5 text-lg mb-2>Composition API</h5>
<div text-sm leading-normal>
  With Composition API, we define a component's logic using imported API functions. In SFCs, Composition API is typically used with <code text-emerald-400>&lt;script setup&gt;</code>. The <code text-emerald-400>setup</code> attribute is a hint that makes Vue perform compile-time transforms that allow us to use Composition API with less boilerplate. For example, imports and top-level variables / functions declared in <code text-emerald-400>&lt;script setup&gt;</code> are directly usable in the template.
</div>
<div>
  Here is the same component, with the exact same template, but using Composition API and <code text-emerald-400>&lt;script setup&gt;</code> instead:
</div>
<<< @/snippets/APIStyle-CompositionAPI.vue vue
</div>
</div>
---
layout: full
glowX: 100
glowY: 50
---

<h2 mb-4>Introduction</h2>
<h3 mb-2>Which to Choose?</h3>

<div text-sm leading-normal max-h-300px overflow-auto my-4 flex="~ col gap-2">
<div>Both API styles are fully capable of covering common use cases. They are different interfaces powered by the exact same underlying system. In fact, the Options API is implemented on top of the Composition API! The fundamental concepts and knowledge about Vue are shared across the two styles.</div>

<div>The Options API is centered around the concept of a "component instance" (this as seen in the example), which typically aligns better with a class-based mental model for users coming from OOP language backgrounds. It is also more beginner-friendly by abstracting away the reactivity details and enforcing code organization via option groups.</div>

<div>The Composition API is centered around declaring reactive state variables directly in a function scope and composing state from multiple functions together to handle complexity. It is more free-form and requires an understanding of how reactivity works in Vue to be used effectively. In return, its flexibility enables more powerful patterns for organizing and reusing logic.</div>

<div>You can learn more about the comparison between the two styles and the potential benefits of Composition API in the <a text-emerald-400 target="_blank" href="https://vuejs.org/guide/extras/composition-api-faq.html">Composition API FAQ</a>.</div>

<div>If you are new to Vue, here's our general recommendation:</div>

<div>For learning purposes, go with the style that looks easier to understand to you. Again, most of the core concepts are shared between the two styles. You can always pick up the other style later.</div>

<div>For production use:</div>

<ul>
  <li>Go with Options API if you are not using build tools, or plan to use Vue primarily in low-complexity scenarios, e.g. progressive enhancement.</li>

  <li>Go with Composition API + Single-File Components if you plan to build full applications with Vue.</li>
</ul>
</div>
---
layout: full
glowX: 50
glowY: 100
---

<h2 mb-4>Quick Start</h2>
<div text-sm leading-normal max-h-300px overflow-auto my-4 flex="~ col gap-2">
<h3>Try Vue Online</h3>
<ul>
  <li>To quickly get a taste of Vue, you can try it directly in our <a href="https://play.vuejs.org/#eNo9jcEKwjAMhl/lt5fpQYfXUQfefAMvvRQbddC1pUuHUPrudg4HIcmXjyRZXEM4zYlEJ+T0iEPgXjn6BB8Zhp46WUZWDjCa9f6w9kAkTtH9CRinV4fmRtZ63H20Ztesqiylphqy3R5UYBqD1UyVAPk+9zkvV1CKbCv9poMLiTEfR2/IXpSoXomqZLtti/IFwVtA9A==" target="_blank" text-emerald-400 inline-flex items-center gap-1><span i-material-symbols:play-circle-outline-rounded text-emerald-400 /> Playground</a></li>

  <li>If you prefer a plain HTML setup without any build steps, you can use this <a href="https://jsfiddle.net/yyx990803/2ke1ab0z/" target="_blank" text-emerald-400>JSFiddle</a> as your starting point.</li>

  <li>If you are already familiar with Node.js and the concept of build tools, you can also try a complete build setup right within your browser on <a href="https://vite.new/vue" target="_blank" text-emerald-400>StackBlitz</a></li>
</ul>
</div>
---
layout: full
glowX: 50
glowY: 100
---

<h2 mb-4>Quick Start</h2>
<div text-sm leading-normal max-h-500px overflow-auto my-4 flex="~ col gap-2">
<h3>Creating a Vue Application</h3>
<div class="border border-emerald-400 p-4 rounded-md">
  <div text-base flex gap-2 items-center text-emerald-400>
    <span i-mdi:information-outline /> <span>Prerequisites</span>
  </div>

  <ul ml-3>
    <li>Familiarity with the command line</li>
    <li>Install Node.js version 18.3 or higher</li>
  </ul>
</div>
<div>In this section we will introduce how to scaffold a <a target="_blank" text-emerald-400 href="https://vuejs.org/guide/extras/ways-of-using-vue.html#single-page-application-spa">Vue Single Page Application</a> on your local machine. The created project will be using a build setup based on <a target="_blank" text-emerald-400 href="https://vitejs.dev/">Vite</a> and allow us to use <a target="_blank" text-emerald-400 href="https://vuejs.org/guide/scaling-up/sfc.html">Vue Single-File Components</a> (SFCs).</div>

<div>Make sure you have an up-to-date version of <a target="_blank" text-emerald-400 href="https://nodejs.org/">Node.js</a> installed and your current working directory is the one where you intend to create a project. Run the following command in your command line</div>
<ul p-0 m-0 class="list-none">
  <li flex items-center gap-2 v-click>
  <code text-emerald-400>npm</code>:
```bash
npm create vue@latest
```
  </li>
  <li flex items-center gap-2 v-click>
  <code text-emerald-400>pnpm</code>:
```bash
pnpm create vue@latest
```
  </li>
  <li flex items-center gap-2 v-click>
  <code text-emerald-400>yarn</code>:
For Yarn Modern (v2+)
```bash
yarn create vue@latest
```
For Yarn ^v4.11
```bash
yarn dlx create-vue@latest
```

  </li>
</ul>
</div>

<style scoped>
  ul.list-none {
    list-style: none;
  }
  ul.list-none li {
    margin: 0px;
    padding: 0px;
  }
</style>

---
layout: center
glowX: 50
glowY: 50
---

<h1 font-bold class="text-5xl!">Developer Experience</h1>

<div absolute left-100 top-80 v-click>File-based Routing</div>
<div absolute left-52 top-50 v-click>Modules Ecosystem</div>
<div absolute left-100 top-50 v-click>Hot Module Replacement</div>
<div absolute left-50 top-80 v-click>Server-side Rendering</div>

<v-click>

<div absolute left-158 top-50>Nitro</div>
<div absolute left-145 top-80>ESM First</div>
<div absolute left-170 top-80>Vite Powered</div>
<div absolute left-60 top-90 op80>Zero-config</div>
<div absolute left-90 top-90>Edge Rendering</div>

</v-click>
<v-click>

<div absolute left-85 top-40>Hybrid Rendering</div>
<div absolute left-130 top-90>Components Auto Imports</div>
<div absolute left-125 top-40 op70>Composables Auto Imports</div>
<div absolute left-55 top-40 op70>Middleware</div>
<div absolute left-175 top-50 op70>SEO</div>

</v-click>
<v-click>

<div absolute left-145 top-100 op60>Server API</div>
<div absolute left-100 top-30 op70>Serverless</div>
<div absolute left-70 top-30 op70>TypeScript</div>
<div absolute left-130 top-30 op70>Server Components</div>
<div absolute left-120 top-100 op70>Layouts</div>
<div absolute left-70 top-100 op60>Static Site Generation</div>

</v-click>

---
glowX: 0
glowY: 50
class: flex
---

<div my-auto w-full grid="~ cols-2 gap-5" px20>
<div flex="~ col gap-5">
<h1 v-click>Conventions</h1>
<h1 v-click>Abstractions</h1>
<h1 v-click>Sensible Defaults</h1>
<h1 v-click>Normalizations</h1>
</div>
<div flex="~ gap-5 items-center">
<h1 v-click class="text-right" w-full>Transparency</h1>
</div>
</div>

---
glowX: 50
glowY: -80
glowSize: 2
class: h-full flex flex-col justify-center
---

# Transparency

<v-clicks>

- Easy to learn & understand

- Easy to modify

- Easy to debug

</v-clicks>

---
layout: 'center'
class: 'text-center'
glowX: 50
glowY: 10
---

<div v-click transition-all duration-500 :class="$clicks === 0 ? 'op0' : $clicks > 1 ? 'op50 text-2xl' : 'translate-y-10 text-4xl'">Introducing</div>

<div class="nuxt-devtools-logo" v-click>
  <NuxtDevTools h-20/>
</div>

---

<div ml-14 text-lg op50 mb--4>The goal of</div>
<h1><NuxtDevTools h-15/></h1>

<div text-2xl>
<v-clicks>

- Enhance your DX with Nuxt

- Improve Transparency

- Performance & analysis

- Interactive & playful

- Personalized documentations

</v-clicks>
</div>

---
layout: center
class: text-center
glowX: 50
glowY: 50
glowSize: 0.4
---

<h1>Demo time!</h1>

---
layout: center
class: text-center
glowX: 50
glowY: 0
---

---
layout: center
class: text-center
glowX: 10
glowY: 90
---

# Open Sourced at

<Repo name="nuxt/devtools" />

---
layout: center
class: text-center
glowX: 50
glowY: -20
---

# Q&A

---
layout: intro
class: text-center pb-5
glowX: 50
glowY: 120
---

# Thank You!

Slides on [antfu.me](https://antfu.me)
