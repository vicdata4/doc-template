<template>
  <div>
    <custom-header></custom-header>
    <main>
      <section aria-label="About dsign project" tabindex="0">
          <div class="information">
            <img class="main-icon" src="../assets/seed-logo.png" width="400">
            <p class="info-text center" tabindex="0">
             An open-source <b>web-components</b> library which contains standards-based web templates such as carousel, modal, dropdown and other interface components.
              </p>
              <NuxtLink to="/seed" class="menu-start">Get Started v1.0</NuxtLink>
            <div style="margin: 60px 0;">
              <hr class="separator centered">
            </div>
          </div>
        </section>
        <section aria-label="Web design disciplines" tabindex="0">
          <div class="areas">
            <article class="area-card">
              <h2 class="area-title" tabindex="0">Custom Elements</h2>
              <p class="info-text" tabindex="0">
                One of the key features of the <b>Web Components standard</b> is the ability to create custom elements that encapsulate your functionality on an HTML page, rather than having to make do with a long, nested batch of elements that together provide a custom page feature.
              </p>
              <a href="https://developer.mozilla.org/en-US/docs/Web/Web_Components/Using_custom_elements" target="_blank">More</a>
            </article>
            <article class="area-card center">
              <h2 class="area-title" tabindex="0">Shadow DOM</h2>
              <p class="info-text" tabindex="0">
                An important aspect of web components is encapsulation — being able to keep the <b>markup structure, style, and behavior hidden and separate</b> from other code on the page so that different parts do not clash, and the code can be kept nice and clean. The Shadow DOM API is a key part of this, providing a way to attach a hidden separated DOM to an element.
              </p>
              <a href="https://developer.mozilla.org/en-US/docs/Web/Web_Components/Using_shadow_DOM" target="_blank">More</a>
            </article>
            <article class="area-card">
              <h2 class="area-title" tabindex="0">HTML templates</h2>
              <p class="info-text" tabindex="0">
                When you have to reuse the same markup structures repeatedly on a web page, it makes sense to use some kind of a template rather than repeating the same structure over and over again. This was possible before, but it is made a lot easier by the HTML <b>&lt;template&gt;</b> element (which is well-supported in modern browsers). This element and its contents are not rendered in the DOM, but it can still be referenced using JavaScript.
              </p>
              <a href="https://developer.mozilla.org/en-US/docs/Web/Web_Components/Using_templates_and_slots" target="_blank">More</a>
            </article>
          </div>
        </section>
        <footer aria-label="Footer section" tabindex="0">
          <ul class="footer-list">
            <li class="footer-link t" aria-label="Menu links" tabindex="0">COMPONENTS</li>
            <li><NuxtLink class="footer-link" to="/seed/carousel">Carousel</NuxtLink></li>
            <li><NuxtLink class="footer-link" to="/seed/mmodal">Modal</NuxtLink></li>
            <li><NuxtLink class="footer-link" to="/seed/dropdown">Dropdown</NuxtLink></li>
            <li><NuxtLink class="footer-link" to="/seed/ring">Ring</NuxtLink></li>
            <li><NuxtLink class="footer-link" to="/seed/stepper">Stepper</NuxtLink></li>
          </ul>
          <ul class="footer-list">
            <li class="footer-link t" aria-label="Technologies links" tabindex="0">TECHNOLOGIES</li>
            <li><a href="https://developer.mozilla.org/en-US/docs/Glossary/HTML5" class="footer-link" target="_blank">HTML5</a></li>
            <li><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript" class="footer-link" target="_blank">Javascript</a></li>
            <li><a href="https://developer.mozilla.org/en-US/docs/Web/CSS" class="footer-link" target="_blank">CSS3</a></li>
            <li><a href="https://developer.mozilla.org/en-US/docs/Web/Web_Components" class="footer-link" target="_blank">Web Components</a></li>
          </ul>
          <ul class="footer-list">
            <li class="footer-link t" aria-label="Dependencies links" tabindex="0">DEPENDENCIES</li>
            <li><a href="https://lit.dev/" class="footer-link" target="_blank">LitElement</a></li>
            <li><a href="https://karma-runner.github.io/latest/index.html" class="footer-link" target="_blank">Karma</a></li>
            <li><a href="https://mochajs.org/" class="footer-link" target="_blank">Mocha</a></li>
            <li><a href="https://www.chaijs.com/" class="footer-link" target="_blank">Chai</a></li>
          </ul>
          <ul class="footer-list">
            <li class="footer-link t" aria-label="Recomendations links" tabindex="0">RELATED</li>
            <li><a href="https://lit.dev/" class="footer-link" target="_blank">Lit</a></li>
            <li><a href="https://github.com/vicdata4/seed-catalog" class="footer-link" target="_blank">Github</a></li>
            <li><a href="https://www.npmjs.com/~vicdata" class="footer-link" target="_blank">Npm</a></li>
          </ul>
        </footer>
      </main>
  </div>
</template>

<script>

import '/components/custom-header';

export default {}
</script>

<style>
@import 'assets/styles/main.css';
@import 'assets/styles/info.css';
@import 'assets/styles/area.css';
@import 'assets/styles/footer.css';

</style>
