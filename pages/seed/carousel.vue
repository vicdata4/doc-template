<template>
  <div>
    <h1 class="title">Carousel</h1>
    <p class="info-text sm" tabindex="0">Install via npm</p>
    <pre><code class="language-bash">{{`npm i @seed-catalog/carousel`}}</code></pre>
    <p class="info-text sm" tabindex="0">Import</p>
    <pre><code class="language-js">{{`import '@seed-catalog/carousel';`}}</code></pre>
    <p class="info-text sm mt" tabindex="0">Properties and attributes</p>
    <div class="mb">
      <p class="info-text sm"><span class="prop-light">speed</span>: type Number</p>
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
  </pre>
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
  <seed-carousel class="carousel-width">
    <img src="https://source.unsplash.com/1600x900/?random" alt="carousel3">
    <img src="https://source.unsplash.com/1600x900/?nature" alt="carousel1">
    <img src="https://source.unsplash.com/1600x900/?water" alt="carousel2">
    <img src="https://source.unsplash.com/1600x900/?nature,water" alt="carousel4">
    <seed-stepper slot="stepper" colorActive="#2dabb4" colorBack="#2dabb445"></seed-stepper>
  </seed-carousel>
  </div>
</template>

<script>
import "@seed-catalog/carousel";
import "@seed-catalog/stepper";
import { pageInit } from '/components/utils/functions';

export default {
  layout: 'seed',
  mounted() {
    pageInit();
  },
};
</script>

<style scoped>

seed-carousel > img {
  width: 100%;
}
</style>
