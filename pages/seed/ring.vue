<template>
  <div>
    <h1 class="title">Progress ring</h1>
    <p class="info-text sm" tabindex="0">Install via <a href="https://www.npmjs.com/package/@seed-catalog/progress-ring" target="_blank">npm</a></p>
    <pre><code class="language-bash">{{`npm i @seed-catalog/progress-ring`}}</code></pre>
    <p class="info-text sm" tabindex="0">Import</p>
    <pre><code class="language-js">{{`import '@seed-catalog/progress-ring';`}}</code></pre>
    <p class="info-text sm mt" tabindex="0">Properties and attributes</p>
    <div class="mb">
      <p class="info-text sm"><span class="prop-light">percent</span>: type Number</p>
      <p class="info-text sm"><span class="prop-light">ringColor</span>: type String</p>
      <p class="info-text sm"><span class="prop-light">text</span>: type String</p>
      <p class="info-text sm"><span class="prop-light">ringColor</span>: type String</p>
      <p class="info-text sm"><span class="prop-light">ringBackground</span>: type String</p>
      <p class="info-text sm"><span class="prop-light">only-text</span>: type Boolean</p>
      <p class="info-text sm"><span class="prop-light">custom</span>: type Boolean</p>
    </div>
    <p class="info-text sm" tabindex="0">Code</p>
    <pre class="line-numbers language-markup">
  <code>&lt;seed-progress-ring percent="20" ringColor="#f70bdd"&gt;</code><code>&lt;/seed-progress-ring&gt;</code>
  </pre>

    <pre class="line-numbers language-markup">
  <code>&lt;seed-progress-ring custom&gt;</code>
    <code>&lt;div slot="custom"&gt;</code>
      ...
    <code>&lt;/div&gt;</code>
  <code>&lt;/seed-progress-ring&gt;</code>
  </pre>
  <p class="info-text sm" tabindex="0">Custom</p>
  <pre class="line-numbers language-markup">
  <code>&lt;seed-progress-ring
    percent="20"
    ringColor="#f70bdd"
    text="Uploading"
    ringBackground="rgba(0, 0, 0, 0.3)"
    background="grey"
    only-text
  &gt;</code><code>&lt;/seed-progress-ring&gt;</code>
  </pre>
  <p class="info-text sm" tabindex="0">Examples</p>
  <seed-progress-ring 
      percent="0"
      textColor="black"
      ringColor="#20abf9"
      ringBackground="rgba(0, 0, 0, 0.3)">
    </seed-progress-ring>
  <seed-progress-ring 
      percent="20"
      textColor="black"
      ringColor="#20abf9"
      ringBackground="rgba(0, 0, 0, 0.3)">
    </seed-progress-ring>
    <seed-progress-ring 
      percent="50"
      textColor="black"
      ringColor="#20abf9"
      ringBackground="rgba(0, 0, 0, 0.3)">
    </seed-progress-ring>
    <seed-progress-ring 
      percent="80"
      textColor="black"
      ringColor="#20abf9"
      ringBackground="rgba(0, 0, 0, 0.3)">
    </seed-progress-ring>
    <seed-progress-ring 
      percent="100"
      textColor="black"
      ringColor="#20abf9"
      ringBackground="rgba(0, 0, 0, 0.3)">
    </seed-progress-ring>
  </div>
</template>

<script>
import "@seed-catalog/progress-ring";
import { pageInit } from '/components/utils/functions';

export default {
  layout: 'seed',
  mounted() {
    pageInit();
  },
};
</script>