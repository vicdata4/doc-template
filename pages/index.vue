<template>
  <div>
    <custom-header></custom-header>
    <main>
      <section aria-label="About dsign project" tabindex="0">
          <div class="information">
            <img class="main-icon" src="../assets/seed-logo.png" width="400">
            <p class="info-text center" tabindex="0">
             An open-source <b>web-components</b> library which contains CSS-styles and standards-based web templates such as buttons, modals, dropdowns and other interface components.
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
              <h2 class="area-title" tabindex="0">Styles</h2>
              <p class="info-text" tabindex="0">
                User experience (UX) is a <b>person's emotions and attitudes about using a particular product</b>, system or service. 
                It includes the practical, experiential, affective, meaningful and valuable aspects of human–computer interaction 
                and product ownership. <br><br>Additionally, it includes a person's perceptions of system aspects such as utility, ease of use and efficiency. </p>
            </article>
            <article class="area-card center">
              <h2 class="area-title" tabindex="0">Components</h2>
              <p class="info-text" tabindex="0">Web accessibility is the inclusive practice of <b>ensuring there are no barriers</b> that prevent interaction with, 
                or access to, websites on the World Wide Web <b>by people with physical disabilities, situational disabilities, and socio-economic 
                restrictions on bandwidth and speed.</b> <br><br>When sites are correctly designed, developed and edited, generally all users have equal 
                access to information and functionality.</p>
            </article>
            <article class="area-card">
              <h2 class="area-title" tabindex="0">Docs</h2>
              <p class="info-text" tabindex="0">The user interface (UI), in the industrial design field of human-computer interaction, is the <b>space where 
                interactions between humans and machines occur.</b> <br><br>The goal of this interaction is to allow effective operation and control of 
                the machine from the human end, whilst the machine simultaneously feeds back information that aids the operators' decision-making 
                process. </p>
            </article>
          </div>
        </section>
        <footer aria-label="Footer section" tabindex="0">
          <ul class="footer-list">
            <li class="footer-link title" aria-label="Menu links" tabindex="0">CONTINENTS</li>
            <li><a href="#" class="footer-link">Africa</a></li>
            <li><a href="#" class="footer-link">Europe</a></li>
            <li><a href="#" class="footer-link">Asia</a></li>
            <li><a href="#" class="footer-link">America</a></li>
            <li><a href="#" class="footer-link">Antarctica</a></li>
            <li><a href="#" class="footer-link">Oceania</a></li>
          </ul>
          <ul class="footer-list">
            <li class="footer-link title" aria-label="Technologies links" tabindex="0">TECHNOLOGIES</li>
            <li><a href="#" class="footer-link">HTML5</a></li>
            <li><a href="#" class="footer-link">CSS3</a></li>
            <li><a href="#" class="footer-link">Javascript</a></li>
          </ul>
          <ul class="footer-list">
            <li class="footer-link title" aria-label="Dependencies links" tabindex="0">DEPENDENCIES</li>
            <li><a href="#" class="footer-link">LitElement</a></li>
            <li><a href="#" class="footer-link">Vaadin</a></li>
          </ul>
          <ul class="footer-list">
            <li class="footer-link title" aria-label="Recomendations links" tabindex="0">RELATED</li>
            <li><a href="#" class="footer-link">Git</a></li>
            <li><a href="#" class="footer-link">Flex-box</a></li>
            <li><a href="#" class="footer-link">Grid Layout</a></li>
            <li><a href="#" class="footer-link">ES6</a></li>
            <li><a href="#" class="footer-link">Web Components</a></li>
            <li><a href="#" class="footer-link">Npm</a></li>
          </ul>
          <div class="footer-line" aria-label="Website links" tabindex="0">
            <a href="#" class="footer-link">dsign.website</a>
            <a href="#" class="footer-link">OpenSource</a>
            <a href="#" class="footer-link">github.com/vicdata4</a>
          </div>
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
