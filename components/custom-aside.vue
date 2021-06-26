<template>
  <aside>
    <ul>
      <label><a href="/seed">Quick Start</a></label>
      <label>Styles</label>
      <li>
        <NuxtLink class="link" id="buttons" to="/seed/buttons">Buttons</NuxtLink>
      </li>
      <li><NuxtLink class="link" id="icons" to="/seed/icons">Icons</NuxtLink></li>
      <li id="groups">Groups</li>
      <label>Components</label>
      <li id="carousel">Carousel</li>
      <li id="modal"><NuxtLink class="link" id="icons" to="/seed/modal">Modal</NuxtLink></li>
      <li id="dropdown">Dropdown</li>
      <li id="collapse">Collapse</li>
      <li id="ring">Progress ring</li>
      <li id="stepper">Stepper</li>
      <li id="player">Video player</li>
      <label>Related</label>
      <li>Lit</li>
      <li>Web Components</li>
      <li>Github</li>
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

ul > label:first-child {
  margin-top: 0;
}
</style>
