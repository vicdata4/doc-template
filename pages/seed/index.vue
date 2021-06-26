<template>
  <div>
    <h1 class="title">Quick Start</h1>
    <p class="info-text mb" tabindex="0">
      Before we start using this libray, it is important to know the most important aspects about web components.
    </p>
    <p class="info-text" tabindex="0">
      Web components are a set of web platform APIs that allow you to create new <i>custom</i>, <i>reusable</i>, <i>encapsulated</i> <b>HTML tags</b> to use in web pages and web apps. Custom components and widgets build on the Web Component standards, will work across modern browsers, and <b>can be used with any JavaScript library or framework</b> that works with HTML.
    </p>
    <p class="info-text" tabindex="0">
      <b>Web components</b> are based on existing web standards. Features to support web components are currently being added to the HTML and DOM specs, letting web developers easily extend HTML with new elements with encapsulated styling and custom behavior.
    </p>
    <p class="info-text mb" tabindex="0">
      If you want to learn more about web components specifications, please follow this <a id="buttons" href="https://www.webcomponents.org/introduction" target="_blank">link</a>
    </p>
    <p class="info-text mb" tabindex="0">
      Now you are ready to start using this library, so follow the next steps to know how to install and import a seed catalog component via npm:
    </p>
    <p class="info-text sm" tabindex="0">Install via npm</p>
    <pre><code class="language-bash">{{`npm i @seed-catalog/modal`}}</code></pre>
    <p class="info-text sm" tabindex="0">Import</p>
    <pre><code class="language-js">{{`import '@seed-catalog/modal';`}}</code></pre>
    <p class="info-text sm" tabindex="0">Add to your html template</p>
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
      Learn more about seed-modal
      <NuxtLink id="buttons" to="/seed/modal">here</NuxtLink>
    </p>
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
