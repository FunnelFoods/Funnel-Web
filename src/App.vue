<template>
  <div id="app">
    <nav class="navbar navbar-expand-lg navbar-default" id="navigation-bar">
      <a class="navbar-brand" href="/">
        <img src="./assets/logo.svg" height="25">
      </a>
      <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbar" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse" id="navbar">
        <ul class="mr-auto"></ul>
        <ul class="ml-auto nav justify-content-end" id="nav" >
          <li class="nav-item">
            <router-link class="nav-link" to="/">Home</router-link>
          </li>
         <!-- <li class="nav-item">
            <router-link class="nav-link" to="/about">About</router-link>
          </li>
          <li class="nav-item">
            <router-link class="nav-link" to="/legal">Legal</router-link>
          </li> -->
          <li class="nav-item">
            <router-link class="nav-link" to="/contact">Contact</router-link>
          </li>
        </ul>
      </div>
    </nav>
    <router-view/>
    <footer>
      <div class="row pt-5"></div>
      <div class="pt-5 pb-3">
        <div class="container">
          <div class="row">
            <div class="col-md-6">
              <h3 class="text-left">Want to learn more?</h3>
            </div>
            <div class="col-md-6">
              <!--<button class="btn btn-outline-dark mr-2">
                Get the App
              </button> -->
              <button class="btn btn-outline-dark mr-2">
                  <router-link class="nav-link text-dark text-left px-0" to="/contact">Contact Us</router-link>
              </button>
            </div>
          </div>
        </div>
      </div>
      <div class="container pb-5" id="social-media">
        <div class="row pt-5">
          <div class="col-md-6">
            <h3 class="text-left">FunnelFoods</h3>
            <!--<router-link class="nav-link text-dark text-left px-0" to="/about">About</router-link>
            <router-link class="nav-link text-dark text-left px-0" to="/legal">Legal</router-link>-->
            <router-link class="nav-link text-dark text-left px-0" to="/contact">Contact</router-link>
          </div>
          <div class="col-md-6">
            <h3 class="text-left">Show us what you create:</h3>
            <div class="overflow-hidden">
              <a href="https://www.linkedin.com/company/funnelfoods"><img src="./assets/linkedin.svg" width="50" class="float-left mr-4" alt="LinkedIn"></a>
              <a href="https://www.facebook.com/FunnelFoods/"><img src="./assets/fb.svg" width="50" class="float-left mr-4" alt="Facebook"></a>
              <a href="https://www.f6s.com/funnelfoods"><img src="./assets/f6s.svg" width="50" class="float-left mr-4" alt="F6S"></a>
            </div>
          </div>
        </div>
      </div>
      <div class="container pb-5 col-12" id="copyright">
        <div class="container pb5">
          <p class="text-left">&copy; FunnelFoods 2019</p>
        </div>
      </div>
    </footer>
  </div>
</template>

<style lang="scss">
  @import 'custom';
  @import '../node_modules/bootstrap/scss/bootstrap.scss';

  @font-face {
    font-family: 'Filson Soft';
    src: url("./fonts/Filson Soft Regular.otf") format('opentype');
  }

  #app {
    font-family: 'Avenir', Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2c3e50;
    /*margin-top: 60px;*/
  }

  .navbar-brand {
    position: relative;
    top: -2px;
    left: 0px;
  }

  .background-svg {
    position: absolute;
    left: 0px;
    top: 0px;
    z-index: -1;
  }

  .background-svg-footer {
    position: relative;
    z-index: -1;
    left: 0px;
  }

  .nav-link {
    color: rgba(255, 255, 255, 1);
    &:hover {
      color: rgba(255, 255, 255, 0.5);
    }
  }

  .nav-item {
    font-size: 1.2em;
  }

  footer {
    background-size: cover;
    background-image: url("./assets/footer-background.svg");
    background-repeat: repeat-x;
    box-shadow: 0 50vh 0 50vh #fadcd2;
  }

  .navbar-toggler {
    background-image: url("data:image/svg+xml;charset=utf8,%3Csvg viewBox='0 0 32 32' xmlns='http://www.w3.org/2000/svg'%3E%3Cpath stroke='rgba(255,255,255, 1)' stroke-width='2' stroke-linecap='round' stroke-miterlimit='10' d='M4 8h24M4 16h24M4 24h24'/%3E%3C/svg%3E");
    background-repeat: no-repeat;
    width: 40px!important;
  }

  .btn {
    border-radius: 50px!important;
  }

  #social-media {
    border-top: solid;
  }

  #copyright {
    background-color: #FADCD2;
    width: 100vw;
    display: block;
  }
</style>
