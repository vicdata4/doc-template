<template>
  <div>
    <h1 class="title">Stepper</h1>
    <p class="info-text sm" tabindex="0">Install via <a href="https://www.npmjs.com/package/@seed-catalog/stepper" target="_blank">npm</a></p>
    <pre><code class="language-bash">{{`npm i @seed-catalog/stepper`}}</code></pre>
    <p class="info-text sm" tabindex="0">Import</p>
    <pre><code class="language-js">{{`import '@seed-catalog/stepper';`}}</code></pre>
    <p class="info-text sm mt" tabindex="0">Properties and attributes</p>
    <div class="mb">
      <p class="info-text sm"><span class="prop-light">index</span>: type Number</p>
      <p class="info-text sm"><span class="prop-light">size</span>: type Number</p>
      <p class="info-text sm"><span class="prop-light">colorActive</span>: type String</p>
      <p class="info-text sm"><span class="prop-light">colorBack</span>: type String</p>
    </div>
    <p class="info-text sm" tabindex="0">Code</p>
    <pre class="line-numbers language-markup">
  <code>&lt;seed-stepper index="1" size="5"&gt;</code><code>&lt;/seed-stepper&gt;</code>
  </pre>
  <p class="info-text sm" tabindex="0">Custom</p>
  <pre class="line-numbers language-markup">
  <code>&lt;seed-stepper index="1" size="5" colorActive="#5e5e5e" colorBack="#a9aaaa45"&gt;</code><code>&lt;/seed-stepper&gt;</code>
  </pre>
  <p class="info-text sm" tabindex="0">Examples</p>
  <seed-stepper index="0" size="5" colorActive="#5e5e5e" colorBack="#a9aaaa45"></seed-stepper>
  <seed-stepper index="1" size="5" colorActive="#5e5e5e" colorBack="#a9aaaa45"></seed-stepper>
  <seed-stepper index="2" size="5" colorActive="#5e5e5e" colorBack="#a9aaaa45"></seed-stepper>
  <seed-stepper index="3" size="5" colorActive="#5e5e5e" colorBack="#a9aaaa45"></seed-stepper>
  <seed-stepper index="4" size="5" colorActive="#5e5e5e" colorBack="#a9aaaa45"></seed-stepper>
  </div>
</template>

<script>
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
  seed-stepper {
    width: fit-content;
  }
</style>
