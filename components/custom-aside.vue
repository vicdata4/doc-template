<template>
  <aside>
    <ul>
      <label><NuxtLink class="link" to="/seed">Quick Start</NuxtLink></label>
      <!--
      <label>Styles</label>
      <li>
        <NuxtLink class="link" to="/seed/buttons">Buttons</NuxtLink>
      </li>
      <li><NuxtLink class="link" to="/seed/icons">Icons</NuxtLink></li>
      <li>Groups</li>
      -->
      <label>Components</label>
      <li><NuxtLink class="link" to="/seed/carousel">Carousel</NuxtLink></li>
      <li>
        <NuxtLink class="link" to="/seed/modal">Modal</NuxtLink>
      </li>
      <li><NuxtLink class="link" to="/seed/dropdown">Dropdown</NuxtLink></li>
      <li><NuxtLink class="link" to="/seed/ring">Ring</NuxtLink></li>
      <li><NuxtLink class="link" to="/seed/stepper">Stepper</NuxtLink></li>
      <label>Related</label>
      <li><a class="link" target="_blank" href="https://lit.dev/">Lit</a></li>
      <li><a class="link" target="_blank" href="https://www.webcomponents.org/introduction">Web Components</a></li>
      <li><a class="link" target="_blank" href="https://github.com/vicdata4/seed-catalog">Github</a></li>
    </ul>
  </aside>
</template>



<style scoped>
ul {
  margin: 0;
  border-right: 1px solid #efe1f6;
  padding: 50px;
  list-style: none;
  background-color: #fdfdfd;
  height: calc(100vh - var(--header-height));
  overflow: auto;
}

ul > li {
  margin-bottom: 20px;
  margin-left: 10px;
}

.link {
  text-decoration: none;
  color: black;
}

.link.active {
  font-weight: bolder;
  color: #1e9fa7 !important;
}

ul > label {
  margin: 30px 0;
  display: block;
  font-weight: bold;
  color: var(--purple-color);
}

ul > label > a {
  color: var(--purple-color);
  text-decoration: none;
}

ul > label > .link {
  color: var(--purple-color) !important;
}

ul > label:first-child {
  margin-top: 0;
}
</style>
