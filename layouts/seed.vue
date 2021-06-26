<template>
  <div>
    <custom-header></custom-header>
    <div class="page-container">
        <custom-aside></custom-aside>
        <div class="section-container">
          <Nuxt />
        </div>
      </div>
  </div>
</template>

<script>
import '/components/custom-header';
import '/components/custom-aside';

export default {}
</script>


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

.page-container {
  display: grid;
  grid-template-columns: 300px 1fr;
  padding-top: var(--header-height);
  overflow: hidden;
}

.section-container {
  padding: 100px 80px;
  height: calc(100vh - var(--header-height));
  overflow: auto;
}

.nuxt-link-active {
    font-weight: bold;
    color: var(--green-color) !important;
}



.title {
  color: #575e64;
  border-bottom: 1px solid #975bb6;
  margin-bottom: 50px;
  padding-bottom: 20px;
  width: 100%
}

 .language-bash, .language-js, .language-markup {
   /*background-color: rgb(236, 240, 241) !important;*/
 }

 .prop-light {
   color: #0677aa;
   font-size: 17px;
 }

 @media (min-width: 1024px) {
  .title {
    width: 50%
  }
}

</style>
