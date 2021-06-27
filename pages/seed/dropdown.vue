<template>
  <div>
    <h1 class="title">Dropdown</h1>
    <p class="info-text sm" tabindex="0">Install via <a href="https://www.npmjs.com/package/@seed-catalog/dropdown" target="_blank">npm</a></p>
    <pre><code class="language-bash">{{`npm i @seed-catalog/dropdown`}}</code></pre>
    <p class="info-text sm" tabindex="0">Import</p>
    <pre><code class="language-js">{{`import '@seed-catalog/dropdown';`}}</code></pre>
    <p class="info-text sm mt" tabindex="0">Properties and attributes</p>
    <div class="mb">
      <p class="info-text sm"><span class="prop-light">clickout</span>: type Boolean</p>
      <p class="info-text sm"><span class="prop-light">maxWidth</span>: type String</p>
      <p class="info-text sm"><span class="prop-light">position</span>: type String</p>
    </div>
    <p class="info-text sm" tabindex="0">Code</p>
    <pre class="line-numbers language-markup">
  <code>&lt;seed-dropdown relative&gt;</code>
    <code>&lt;button slot="button"&gt;</code>Open dropdown<code>&lt;/button&gt;</code>
    <code>&lt;div slot="content"&gt;</code>
      ...
    <code>&lt;/div&gt;</code>
  <code>&lt;/seed-dropdown&gt;</code>
  </pre>
  <p class="info-text sm" tabindex="0">Accordion</p>
  <pre><code class="language-bash">{{`npm i @seed-catalog/collapse`}}</code></pre>
  <pre><code class="language-js">{{`import '@seed-catalog/collapse';`}}</code></pre>
    <pre class="line-numbers language-markup">
  <code>&lt;seed-collapse basic&gt;</code>
    <code>&lt;seed-dropdown relative&gt;</code>
      <code>&lt;button slot="button"&gt;</code>Open dropdown<code>&lt;/button&gt;</code>
      <code>&lt;div slot="content"&gt;</code>
        ...
      <code>&lt;/div&gt;</code>
    <code>&lt;/seed-dropdown&gt;</code>
  <code>&lt;/seed-collapse&gt;</code>
  </pre>
  <p class="info-text sm" tabindex="0">Custom</p>
  <pre class="line-numbers language-markup">
  <code>&lt;seed-dropdown clickout maxWidth="300" position="relative"&gt;</code><code>&lt;/seed-dropdown&gt;</code>
  </pre>
  <p class="info-text sm" tabindex="0">Examples</p>
  <seed-dropdown position="relative">
    <button slot="button">Relative dropdown</button>
    <p slot="content">
      Lorem ipsum dolor sit amet, consectetur adipiscing elit.
      Cras ut viverra leo, vel dapibus quam. Proin a sollicitudin quam,
      eget viverra diam. Donec euismod mattis dignissim.
    </p>
  </seed-dropdown>
  <seed-dropdown>
    <button slot="button">Default</button>
    <div slot="content" style="width: 200px;">
      Lorem ipsum dolor sit amet, consectetur adipiscing elit.
      Cras ut viverra leo, vel dapibus quam. Proin a sollicitudin quam,
      eget viverra diam. Donec euismod mattis dignissim.
    </div>
  </seed-dropdown>
  <seed-dropdown clickout>
    <button slot="button">Clickout</button>
    <div slot="content" style="width: 200px;">
      Lorem ipsum dolor sit amet, consectetur adipiscing elit.
      Cras ut viverra leo, vel dapibus quam. Proin a sollicitudin quam,
      eget viverra diam. Donec euismod mattis dignissim.
    </div>
  </seed-dropdown>
  <p class="info-text sm" tabindex="0">Accordion</p>
  <seed-collapse basic>
  <seed-dropdown position="relative">
    <button slot="button">Accordion</button>
    <div slot="content">
      Lorem ipsum dolor sit amet, consectetur adipiscing elit.
      Cras ut viverra leo, vel dapibus quam. Proin a sollicitudin quam,
      eget viverra diam. Donec euismod mattis dignissim.
    </div>
  </seed-dropdown>
  <seed-dropdown position="relative">
    <button slot="button">Accordion</button>
    <div slot="content">
      Lorem ipsum dolor sit amet, consectetur adipiscing elit.
      Cras ut viverra leo, vel dapibus quam. Proin a sollicitudin quam,
      eget viverra diam. Donec euismod mattis dignissim.
    </div>
  </seed-dropdown>
  <seed-dropdown position="relative">
    <button slot="button">Accordion</button>
    <div slot="content">
      Lorem ipsum dolor sit amet, consectetur adipiscing elit.
      Cras ut viverra leo, vel dapibus quam. Proin a sollicitudin quam,
      eget viverra diam. Donec euismod mattis dignissim.
    </div>
  </seed-dropdown>
  </seed-collapse>
  </div>
</template>

<script>
import "@seed-catalog/dropdown";
import "@seed-catalog/collapse";
import { pageInit } from '/components/utils/functions';

export default {
  layout: 'seed',
  mounted() {
    pageInit();
  },
};
</script>

