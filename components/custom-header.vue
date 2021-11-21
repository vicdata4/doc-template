<template>
  <header>
    <NuxtLink to="/"
      ><img src="../assets/seed-icon.png" class="header-icon" width="30"
    /></NuxtLink>
    <div class="header-menu">
      <NuxtLink to="/seed" :class="`menu-link${homeMenu ? ' home' : ''}`">Components</NuxtLink>
      <button v-if="!homeMenu" class="mobile-menu" @click="openMenu">
        <svg xmlns="http://www.w3.org/2000/svg" enable-background="new 0 0 24 24" height="30px" viewBox="0 0 24 24" width="30px" fill="#5b87b6"><g><rect fill="none" height="24" width="24"/></g><g><g/><g><path d="M21,5c-1.11-0.35-2.33-0.5-3.5-0.5c-1.95,0-4.05,0.4-5.5,1.5c-1.45-1.1-3.55-1.5-5.5-1.5S2.45,4.9,1,6v14.65 c0,0.25,0.25,0.5,0.5,0.5c0.1,0,0.15-0.05,0.25-0.05C3.1,20.45,5.05,20,6.5,20c1.95,0,4.05,0.4,5.5,1.5c1.35-0.85,3.8-1.5,5.5-1.5 c1.65,0,3.35,0.3,4.75,1.05c0.1,0.05,0.15,0.05,0.25,0.05c0.25,0,0.5-0.25,0.5-0.5V6C22.4,5.55,21.75,5.25,21,5z M21,18.5 c-1.1-0.35-2.3-0.5-3.5-0.5c-1.7,0-4.15,0.65-5.5,1.5V8c1.35-0.85,3.8-1.5,5.5-1.5c1.2,0,2.4,0.15,3.5,0.5V18.5z"/><g><path d="M17.5,10.5c0.88,0,1.73,0.09,2.5,0.26V9.24C19.21,9.09,18.36,9,17.5,9c-1.7,0-3.24,0.29-4.5,0.83v1.66 C14.13,10.85,15.7,10.5,17.5,10.5z"/><path d="M13,12.49v1.66c1.13-0.64,2.7-0.99,4.5-0.99c0.88,0,1.73,0.09,2.5,0.26V11.9c-0.79-0.15-1.64-0.24-2.5-0.24 C15.8,11.66,14.26,11.96,13,12.49z"/><path d="M17.5,14.33c-1.7,0-3.24,0.29-4.5,0.83v1.66c1.13-0.64,2.7-0.99,4.5-0.99c0.88,0,1.73,0.09,2.5,0.26v-1.52 C19.21,14.41,18.36,14.33,17.5,14.33z"/></g></g></g></svg>
      </button>
      <a href="https://github.com/vicdata4/seed-catalog" target="_blank"
        ><svg
          xmlns="http://www.w3.org/2000/svg"
          width="24"
          height="24"
          class="github-icon"
          viewBox="0 0 24 24"
        >
          <path
            d="M12 0c-6.626 0-12 5.373-12 12 0 5.302 3.438 9.8 8.207 11.387.599.111.793-.261.793-.577v-2.234c-3.338.726-4.033-1.416-4.033-1.416-.546-1.387-1.333-1.756-1.333-1.756-1.089-.745.083-.729.083-.729 1.205.084 1.839 1.237 1.839 1.237 1.07 1.834 2.807 1.304 3.492.997.107-.775.418-1.305.762-1.604-2.665-.305-5.467-1.334-5.467-5.931 0-1.311.469-2.381 1.236-3.221-.124-.303-.535-1.524.117-3.176 0 0 1.008-.322 3.301 1.23.957-.266 1.983-.399 3.003-.404 1.02.005 2.047.138 3.006.404 2.291-1.552 3.297-1.23 3.297-1.23.653 1.653.242 2.874.118 3.176.77.84 1.235 1.911 1.235 3.221 0 4.609-2.807 5.624-5.479 5.921.43.372.823 1.102.823 2.222v3.293c0 .319.192.694.801.576 4.765-1.589 8.199-6.086 8.199-11.386 0-6.627-5.373-12-12-12z"
          /></svg
      ></a>
    </div>
  </header>
</template>

<script>
export default {
  props: ['homeMenu'],
  methods: {
    openMenu() {
      const menu = document.querySelector('.menu-bar');

      if (!menu.classList.contains('show')) {
        menu.classList.add('show');
      } else {
        menu.classList.remove('show');
      }
    }
  },
};
</script>

<style scoped>
header {
  position: fixed;
  top: 0;
  z-index: 1;

  display: flex;
  align-items: center;
  justify-content: space-between;

  padding: 0 20px;
  width: 100%;
  height: var(--header-height);

  background-color: white;
  border-bottom: 4px solid rgb(235, 235, 235);
}

.menu-link {
  display: none;
  margin-right: 30px;
  text-decoration: none;

  background-color: black;
  color: white;
  padding: 8px 24px;
  border-radius: 4px;
}

.github-icon {
  display: block;
}

.menu-link:hover {
  background-color: #222222;
}

.header-menu {
  display: flex;
  align-items: center;
}

.header-icon {
  display: block;
}

.logo {
  width: 115px;
  height: auto;
}

.nuxt-link-active {
  font-weight: unset;
  color: white !important;
}

.mobile-menu {
  appearance: none;
  background: none;
  border: none;
  margin-right: 30px;
}

.menu-link.home {
  display: block;
}

@media (min-width: 540px) {
  header {
    padding: 0 var(--header-padding);
  }
}

@media (min-width: 1024px) {
.menu-link {
  display: block;
}

.mobile-menu {
  display: none;
}
}
</style>
