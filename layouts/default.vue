<template>
  <div>
    <div class="nav">
        <div><nuxt-link to="/">Home</nuxt-link></div>
        <div>
          <ul>
            <li><nuxt-link to="/blog">Blog</nuxt-link>
            <li><nuxt-link to="/about">About</nuxt-link></li>
          </ul>
        </div>
    </div>
    <Nuxt />
  </div>
</template>

<style>
html {
  font-family:
    'Source Sans Pro',
    -apple-system,
    BlinkMacSystemFont,
    'Segoe UI',
    Roboto,
    'Helvetica Neue',
    Arial,
    sans-serif;
  font-size: 16px;
  word-spacing: 1px;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
}

*,
*::before,
*::after {
  box-sizing: border-box;
  margin: 0;
}

.nav {
  width: 100%;
  height: 4rem;
  background: dodgerblue;
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  align-items: center;
  color: #fff;
  font-size: 1.5rem;
}
.nav ul {
  display: flex;
  flex-direction: row;
  justify-content: space-around;
  width: 10%;
}

.nav li {
  list-style: none;
  margin-right: 1rem;
}

.nav a:link, .nav a:visited {
  color: #fff;
  text-decoration: none;
}
</style>
