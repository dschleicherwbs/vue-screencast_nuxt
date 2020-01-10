<template>
  <div>
    <div id="navbar">
      <div id="navbar__links">
        <nuxt-link to="/">Home</nuxt-link>
        <nuxt-link to="/videos">Videos</nuxt-link>
        <nuxt-link to="/theatre">Theatre</nuxt-link>
      </div>
    </div>
    <div id="main-container">
      <nuxt />
    </div>
  </div>
</template>

<style lang="scss">
html {
  font-family: "Source Sans Pro", -apple-system, BlinkMacSystemFont, "Segoe UI",
    Roboto, "Helvetica Neue", Arial, sans-serif;
  font-size: 16px;
  word-spacing: 1px;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
}

#navbar {
  height: 90px;
  width: 100%;
  background-color: #333;

  display: grid;
  grid-auto-flow: column;
  justify-content: end;
  align-items: center;
}

*,
*:before,
*:after {
  box-sizing: border-box;
  margin: 0;
}

#main-container {
  max-width: 100vw;
  margin-top: 4rem;
}

#navbar__links {
  display: grid;
  grid-auto-flow: column;
  justify-content: end;
  align-items: center;
  gap: 3rem;

  & a,
  & a:visited {
    font-size: 1.4rem;
    color: #fff;
    text-decoration: none;

    &:hover {
      color: yellow;
    }
  }
}

#main-container,
#navbar__links {
  margin-left: 4rem;
  margin-right: 4rem;
}

.button--green {
  display: inline-block;
  border-radius: 4px;
  border: 1px solid #3b8070;
  color: #3b8070;
  text-decoration: none;
  padding: 10px 30px;
}

.button--green:hover {
  color: #fff;
  background-color: #3b8070;
}

.button--grey {
  display: inline-block;
  border-radius: 4px;
  border: 1px solid #35495e;
  color: #35495e;
  text-decoration: none;
  padding: 10px 30px;
  margin-left: 15px;
}

.button--grey:hover {
  color: #fff;
  background-color: #35495e;
}
</style>
