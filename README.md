# Apple Website Clone

## Project Overview
This repository contains the first stage of developing an Apple website clone using React and Tailwind CSS. The project is initialized with Vite as the build tool for its speed and simplicity.

<br>

## Stage 02 : Add Resource 
#### Log: January 8, 2025
<hr>
<br>

### Step-by-Step Process

#### 1. Add colors

```js
 colors: {
        blue: "#2997FF",
        gray: {
          DEFAULT: "#86868b",
          100: "#94928d",
          200: "#afafaf",
          300: "#42424570",
        },
        zinc: "#101010",
      },
```


<details>
<summary><code>tailwind.config.js</code></summary>

<br>

```js
/** @type {import('tailwindcss').Config} */
export default {
  content: ["./index.html", "./src/**/*.{js,ts,jsx,tsx}"],
  theme: {
    extend: {
      colors: {
        blue: "#2997FF",
        gray: {
          DEFAULT: "#86868b",
          100: "#94928d",
          200: "#afafaf",
          300: "#42424570",
        },
        zinc: "#101010",
      },
    },
  },
  plugins: [],
};
```

</details>



#### 2. Update index file with helpers

<details>
<summary><code>index.css</code></summary>

<br>

```css
@tailwind base;
@tailwind components;
@tailwind utilities;

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  color: white;
  width: 100dvw;
  overflow-x: hidden;
  height: 100%;
  background: #000;
  border-color: #3b3b3b;
  user-select: none;
}

canvas {
  touch-action: none;
}

.scrim-max-width {
  margin-inline-start: auto;
  margin-inline-end: auto;
  position: relative;
  max-width: 1120px;
}

@layer utilities {
  .flex-center {
    @apply flex items-center justify-center
  }

  .nav-height {
    @apply h-[calc(100vh-60px)]
  }

  .btn {
    @apply px-5 py-2 rounded-3xl bg-blue my-5 hover:bg-transparent border border-transparent hover:border hover:text-blue hover:border-blue
  }

  .color-container {
    @apply flex items-center justify-center px-4 py-4 rounded-full bg-gray-300 backdrop-blur
  }

  .size-btn-container {
    @apply flex items-center justify-center p-1 rounded-full bg-gray-300 backdrop-blur ml-3 gap-1
  }

  .size-btn {
    @apply w-10 h-10 text-sm flex justify-center items-center bg-white text-black rounded-full transition-all
  }

  .common-padding {
    @apply sm:py-32 py-20 sm:px-10 px-5
  }

  .section-heading {
    @apply text-gray lg:text-6xl md:text-5xl text-3xl lg:mb-0 mb-5 font-medium opacity-0 translate-y-20
  }

  .feature-text {
    @apply text-gray max-w-md text-lg md:text-xl font-semibold opacity-0 translate-y-[100px]
  }

  .feature-text-container {
    @apply w-full flex-center flex-col md:flex-row mt-10 md:mt-16 gap-5
  }

  .feature-video {
    @apply w-full h-full object-cover object-center scale-150 opacity-0
  }

  .feature-video-container {
    @apply w-full flex flex-col md:flex-row gap-5 items-center
  }

  .link {
    @apply text-blue hover:underline cursor-pointer flex items-center text-xl opacity-0 translate-y-20
  }

  .control-btn {
    @apply ml-4 p-4 rounded-full bg-gray-300 backdrop-blur flex-center
  }

  .hero-title {
    @apply text-center font-semibold text-3xl text-gray-100 opacity-0 max-md:mb-10
  }

  .hiw-title {
    @apply text-4xl md:text-7xl font-semibold text-center
  }

  .hiw-subtitle {
    @apply text-gray font-semibold text-xl md:text-2xl py-10 text-center
  }

  .hiw-video {
    @apply absolute w-[95%] h-[90%] rounded-[56px] overflow-hidden
  }

  .hiw-text-container {
    @apply flex md:flex-row flex-col justify-between items-start gap-24
  }

  .hiw-text {
    @apply text-gray text-xl font-normal md:font-semibold
  }

  .hiw-bigtext {
    @apply text-white text-3xl md:text-5xl font-normal md:font-semibold my-2
  }

  .video-carousel_container {
    @apply relative sm:w-[70vw] w-[88vw] md:h-[70vh] sm:h-[50vh] h-[35vh]
  }

  .g_fadeIn {
    @apply opacity-0 translate-y-[100px]
  }
}
```
</details>



#### 3. Add images Assets

first delete assests folder in 'src'

inside 'public' folder create 'assets' folder inside create 'images' & 'videos' folder

add images* (already in this repo)
add videos from below link (couse it is not in this repo)
```
https://drive.google.com/drive/folders/193simR5ud2I4ChhXN8cT-ZMAibI7DMQR?usp=sharing
```


#### 4. Add model Assets
inside 'public' folder create 'model' folder

add scene.glb
(which is already in this repo)






<details>
<summary><code>t</code></summary>

<br>


</details>

