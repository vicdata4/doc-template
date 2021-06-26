<template>
  <div>
    <Nuxt />
  </div>
</template>

<style>
body, html {
  --header-height: 80px;
  --nav-height: 50px;
  --header-padding: 80px;

  --green-color: #1e9fa7;
  --purple-color: rgb(152 90 182);

  --header-background: rgb(50, 50, 50);
  --border-grey: #c7c4c4;
}

html {
  font-family: "Open Sans", sans-serif, Arial;
  font-size: 16px;
  line-height: 1.6;
  letter-spacing: 0.4px;
  font-weight: 300;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  /*-moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;*/
  box-sizing: border-box;
}

*,
*::before,
*::after {
  box-sizing: border-box;
  margin: 0;
}

</style>
