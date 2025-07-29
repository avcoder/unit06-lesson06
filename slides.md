---
# You can also start simply with 'default'
theme: default
# random image from a curated Unsplash collection by Anthony
# like them? see https://unsplash.com/collections/94734566/slidev
background: /assets/intro.jpg
# some information about your slides (markdown enabled)
title: Software Development | Foundations
info: |
  ## Software Development | Foundations
# apply unocss classes to the current slide
class: text-left
drawings:
  persist: false
transition: slide-left
mdc: true
---

# React: UseEffect
Frontend Development: Unit 06 - Lesson 06

- [ ] useEffect for fetching
- [ ] useEffect as a watcher
- [ ] RTK Query vs TanStack Query

<div class="abs-br m-6 text-xl">
  <a href="https://github.com/slidevjs/slidev" target="_blank" class="slidev-icon-btn">
    <carbon:logo-github />
  </a>
</div>

<!--
-->


---
transition: slide-left
---

# Recap
- Let's look again at last week's exercise of [Putting it all together](https://unit06-lesson05.netlify.app/11)
   - 👀 use of TS
   - could have stored all info (name, username, avatar etc.), but for learning purposes only, just chose to store array of type Person:
   ```ts
    export type PersonType = { 
      name: string;
      isFollowing?: boolean 
    }
   ```

---
transition: slide-left
---

# useEffect (pg.1)
Use to update browser tab title


---
transition: slide-left
---

# useEffect (pg.2)
Use to fetch JSON

---
transition: slide-left
---

# useEffect (pg.3)
use as a Watcher


---
layout: image-right
transition: slide-left
image: /assets/ninja.png
backgroundSize: 420px 450px
class: text-left
---

# 10 minute break

🍦 Cool Tips, Trends and Resources:

- 🌊 [useEffect in 60 sec](https://x.com/thenetninjauk/status/1942882433742819389)
- 🎠 https://motion.dev/
- 🕵️ https://testing-library.com/
- 📖 https://storybook.js.org/


<br>
<hr>
<br>

- 🧪 [Enter anonymous lab questions](https://docs.google.com/forms/d/e/1FAIpQLSevvGARdHQikso-uLqFCO481MABKE5HofuSrlzEPMNQ2ZLykw/viewform?usp=dialog)
- ℹ️ [Course feedback survey](https://circuitstream.typeform.com/to/ZoyYk7px#course_id=SoftwareAN&instructor=9514)

---
transition: slide-left
---

# O

---
transition: slide-left
layout: two-cols
---


# Lab tomorrow
Option: Choose a Getting Started Activity, OR ask questions AMA (ex: error handling review)

Do at least 1 "Getting Started" from:
  - [Next JS](https://nextjs.org/docs/app/getting-started/installation)
  - [Astro](https://docs.astro.build/en/tutorial/0-introduction/)
  - [React Server Components](https://react.dev/reference/rsc/server-components)
  - [Electron](https://www.electronjs.org/docs/latest/tutorial/tutorial-first-app)
  - [Tauri](https://v2.tauri.app/)
  - [Storybook](https://storybook.js.org/)
  - [Zod](https://zod.dev/)
  - [Redux](https://redux.js.org/)
  - [Zustand](https://zustand-demo.pmnd.rs/)
  - [shadcdn UI](https://ui.shadcn.com/)


::right::
  - [Auth0](https://auth0.com/t)
  - [RedwoodSDK](https://docs.rwsdk.com/)
  - [Keystone JS](https://keystonejs.com/)
  - [React Testing Library](https://testing-library.com/docs/react-testing-library/intro/)
  - [React PDF](https://react-pdf.org/)
  - [Playwright](https://playwright.dev/)
  - [GrowthBook](https://www.growthbook.io/)
  - [Tanstack Query](https://tanstack.com/query/latest)
  - [Remix](https://remix.run/)
  - [Alpine JS](https://alpinejs.dev/)
  - [HTMX](https://htmx.org/)
  - [VuePress](https://vuepress.vuejs.org/)
  - [Lodash](https://lodash.com/)
  - [Bun](https://bun.com/)
  - or any other tech from job postings / [Unit 4](https://unit04-lesson05.netlify.app/16)

