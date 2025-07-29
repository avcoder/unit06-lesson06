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

- fyi - RSC can be compatible with functional React, but only if backend is node
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

- Q: So we know React is responible for producing UI on the page, but how would we change the browser tab title `document.title = 'Home page'` for example? (since the `<title>` tag falls outside of React's `<div id="root"></div>`)
- Side Effects: anytime we want to do something that's outside of React's responsibilities but we still want synchronized with our React component's state

  ```jsx
  import { useEffect } from 'react'

  useEffect(() => {
    document.title = `Home page`
  });
  ```

---
transition: slide-left
---

# Exercise: useEffect to change document.title

- Refactor our Counter button example such that the browser tab also shows the latest counter


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
transition: slide-left
---

# useEffect (pg.4)
Use to keep track of window's width/height

- in this case, if you `addEventListener` yourself, to prevent memory leaks, you must remember to clean up via `removeEventListener`

```jsx
useEffect(() => {
  const handleResize = () => {
    setWindowSize({ width: window.innerWidth, height: window.innerHeight });
  };

  window.addEventListener('resize', handleResize);
  return () => window.removeEventListener('resize', handleResize);
}, []);
```


---
transition: slide-left
---

# Exercise:

- Create app that displays recipe categories
- Upon clicking a category, app will display recipies related to that category
- Upon clicking a recipe, app will display that recipe

- see https://www.themealdb.com/api.php


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

# RTK Query

- see https://redux-toolkit.js.org/rtk-query/overview

---
transition: slide-left
---

# Tanstack Query

- see https://tanstack.com/query/latest

---
transition: slide-left
---

# Homework

Use `useEffect` to:
- start/show an interval timer (remember to clean up to clear the interval when React component unmounts)
- show if browser is online/offline via checking `navigator.onLine` and `window.addEventListener('online')`
- auto-save form data to localStorage every few seconds or on change
- Start working on your React Weather App assignment

---
transition: slide-left
layout: two-cols
---


# Lab tomorrow
Option: Choose a Getting Started Activity 

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

