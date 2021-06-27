<template>
  <div>
    <h1 class="title">Carousel</h1>
    <p class="info-text sm" tabindex="0">Install via <a href="https://www.npmjs.com/package/@seed-catalog/carousel" target="_blank">npm</a></p>
    <pre><code class="language-bash">{{`npm i @seed-catalog/carousel`}}</code></pre>
    <p class="info-text sm" tabindex="0">Import</p>
    <pre><code class="language-js">{{`import '@seed-catalog/carousel';`}}</code></pre>
    <p class="info-text sm mt" tabindex="0">Properties and attributes</p>
    <div class="mb">
      <p class="info-text sm">
        <span class="prop-light">speed</span>: type Number
      </p>
    </div>
    <p class="info-text sm" tabindex="0">Code</p>
    <pre class="line-numbers language-markup">
  <code>&lt;seed-carousel&gt;</code>
    <code>&lt;div&gt;</code>Card 1<code>&lt;/div&gt;</code>
    <code>&lt;div&gt;</code>Card 2<code>&lt;/div&gt;</code>
    <code>&lt;div&gt;</code>Card 3<code>&lt;/div&gt;</code>
    <code>&lt;div&gt;</code>Card 4<code>&lt;/div&gt;</code>
    <code>&lt;div&gt;</code>Card 5<code>&lt;/div&gt;</code>
  <code>&lt;/seed-carousel&gt;</code>
  </pre
    >
    <pre class="line-numbers language-markup">
  <code>&lt;seed-carousel&gt;</code>
    <code>&lt;div&gt;</code>Card 1<code>&lt;/div&gt;</code>
    <code>&lt;div&gt;</code>Card 2<code>&lt;/div&gt;</code>
    <code>&lt;div&gt;</code>Card 3<code>&lt;/div&gt;</code>
    <code>&lt;seed-stepper slot="stepper"&gt;</code><code>&lt;/seed-stepper&gt;</code>
  <code>&lt;/seed-carousel&gt;</code>
  </pre>
    <p class="info-text sm" tabindex="0">Custom</p>
    <pre class="line-numbers language-markup">
  <code>&lt;seed-carousel speed="${1000}"&gt;</code><code>&lt;/seed-carousel&gt;</code>
  </pre>
    <p class="info-text sm" tabindex="0">Examples</p>
    <seed-carousel>
      <img src="https://source.unsplash.com/1600x900/?random" alt="carousel3" />
      <img src="https://source.unsplash.com/1600x900/?nature" alt="carousel1" />
      <img src="https://source.unsplash.com/1600x900/?water" alt="carousel2" />
      <img
        src="https://source.unsplash.com/1600x900/?nature,water"
        alt="carousel4"
      />
      <seed-stepper
        slot="stepper"
        colorActive="#5e5e5e"
        colorBack="#a9aaaa45"
      ></seed-stepper>
    </seed-carousel>

    <div class="carousel-container">
      <seed-carousel>
        <div class="card bl-u"></div>
        <div class="card oran-g"></div>
        <div class="card gre-e"></div>
        <div class="card purp-l"></div>
        <seed-stepper
          slot="stepper"
          colorActive="#5e5e5e"
          colorBack="#a9aaaa45"
        ></seed-stepper>
      </seed-carousel>
    </div>
  </div>
</template>

<script>
import "@seed-catalog/carousel";
import "@seed-catalog/stepper";
import { pageInit } from "/components/utils/functions";

export default {
  layout: "seed",
  mounted() {
    pageInit();
  },
};
</script>

<style scoped>
seed-carousel > img {
  width: 100%;
}

.card {
  min-width: 328px;
  height: 530px;
}

.bl-u {
  background-color: #43aad7;
}

.oran-g {
  background-color: #e18b46;
}

.gre-e {
  background-color: #5dbe59;
}

.purp-l {
  background-color: #b250b2;
}

@media screen and (min-width: 768px) {
  .carousel-container {
    max-width: 500px;
  }
}
</style>
