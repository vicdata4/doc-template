<template>
  <div>
    <h1 class="title">Quick Start</h1>
    <p class="info-text mb" tabindex="0">
      User experience (UX) is a
      <b>person's emotions and attitudes about using a particular product</b>,
      system or service. It includes the practical, experiential, affective,
      meaningful and valuable aspects of human–computer interaction and product
      ownership.
    </p>
    <p class="info-text sm" tabindex="0">Install via npm</p>
    <pre><code class="language-bash">{{`npm i @seed-catalog/modal`}}</code></pre>
    <p class="info-text sm" tabindex="0">Import to your .js file</p>
    <pre><code class="language-js">{{`import '@seed-catalog/modal';`}}</code></pre>
    <p class="info-text sm" tabindex="0">Add to your .html</p>
    <pre class="line-numbers language-markup">
  <code>&lt;seed-modal&gt;</code>
    <code>&lt;button slot="button"&gt;</code>Open modal<code>&lt;/button&gt;</code>
    <code>&lt;div slot="header"&gt;</code>
      <code>&lt;button class="close"&gt;</code>Close modal<code>&lt;/button&gt;</code>
    <code>&lt;/div&gt;</code>
    <code>&lt;div slot="content"&gt;</code>
      ...
    <code>&lt;/div&gt;</code>
    <code>&lt;div slot="footer"&gt;</code>
      <code>&lt;button class="close"&gt;</code>Close modal<code>&lt;/button&gt;</code>
    <code>&lt;/div&gt;</code>
  <code>&lt;/seed-modal&gt;</code>
  </pre>
    <p class="info-text sm" tabindex="0">Result</p>
    <seed-modal>
      <button slot="button" class="sd-btn blue">Default Modal</button>
      <div slot="header" class="header">
        <button class="close">Close modal</button>
      </div>
      <div slot="content">
        Lorem ipsum dolor sit amet, consectetur adipiscing elit.
      </div>
      <div slot="footer" class="footer">
        <button class="close">Close modal</button>
      </div>
    </seed-modal>
    <seed-modal centered>
      <button slot="button" class="sd-btn blue">Centered Modal</button>
      <div slot="header" class="header">
        <button class="close">Close modal</button>
      </div>
      <div slot="content">
        Lorem ipsum dolor sit amet, consectetur adipiscing elit.
      </div>
      <div slot="footer" class="footer">
        <button class="close">Close modal</button>
      </div>
    </seed-modal>
    <p class="info-text sm" tabindex="0">
      Lear more about seed-modal
      <NuxtLink id="buttons" to="/seed/modal">here</NuxtLink>
    </p>
  </div>
</template>

<script>
import "static/utils/prism";
import "@seed-catalog/modal";

export default {
  layout: "seed",
  mounted() {
    Prism.highlightAll();
  },
};
</script>

<style>
</style>
