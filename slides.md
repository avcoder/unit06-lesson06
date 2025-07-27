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

# useEffect

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
---

# Homework

- Refactor the weather app we did for our first exercise (see https://codepen.io/codevilla/pen/YPyWWpm) into the following components.  Then separate the css into its respective components that you created.
Feel free to create more components inside `<Forecast>` as you see fit.  FYI - ignore my `this.whatever` or `this.state.whatever` code below since I was using class-based React which you won't be using.
  ```jsx
  return (
      <div>
        <header>
          <Nav city={this.state.currentCity} handleCityChange={this.changeCity} />
        </header>
        <main>
          <TodayWeather
            city={this.state.currentCity}
            handleCoordsChange={this.changeCoords}
          />
          <Forecast lat={this.state.lat} lon={this.state.lon} />
        </main>
      </div>
    );
  ```
- Start working on "Weather Forecasting App" assignment due Aug 17 midnight EST
