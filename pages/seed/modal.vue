<template>
  <div>
    <h1 class="title">Modal</h1>
    <p class="info-text sm" tabindex="0">Install via <a href="https://www.npmjs.com/package/@seed-catalog/modal" target="_blank">npm</a></p>
    <pre><code class="language-bash">{{`npm i @seed-catalog/modal`}}</code></pre>
    <p class="info-text sm" tabindex="0">Import</p>
    <pre><code class="language-js">{{`import '@seed-catalog/modal';`}}</code></pre>
    <p class="info-text sm mt" tabindex="0">Properties and attributes</p>
    <div class="mb">
      <p class="info-text sm"><span class="prop-light">hide-click-out</span>: type Boolean</p>
      <p class="info-text sm"><span class="prop-light">no-styles</span>: type Boolean</p>
      <p class="info-text sm"><span class="prop-light">centered</span>: type Boolean</p>
      <p class="info-text sm"><span class="prop-light">modalBackground</span>: type String</p>
    </div>
    <p class="info-text sm" tabindex="0">Code</p>
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
  <p class="info-text sm" tabindex="0">Custom</p>
  <pre class="line-numbers language-markup">
  <code>&lt;seed-modal hide-click-out centered no-styles modalBackground="green"&gt;</code><code>&lt;/seed-modal&gt;</code>
  </pre>
  <p class="info-text sm" tabindex="0">Examples</p>
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
    <seed-modal hide-click-out>
      <button slot="button" class="sd-btn blue">Hide clickout</button>
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
    <seed-modal no-styles>
      <button slot="button" class="sd-btn blue">No styles</button>
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
    <seed-modal modalBackground="#44849cb5">
      <button slot="button" class="sd-btn blue">Modal background</button>
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
  </div>
</template>

<script>
import "@seed-catalog/modal";
import { pageInit } from '/components/utils/functions';

export default {
  layout: 'seed',
  mounted() {
    pageInit();
  },
};
</script>

<style>
</style>
