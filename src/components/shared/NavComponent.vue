<template>
  <header>
    <nav class='navbar fixed-top navbar-expand-lg'>
      <!-- Container 1 -->
      <button class='navbar-toggler' type='button' data-toggle='collapse' data-target='#navbar' aria-controls="navbar" aria-expanded="false" aria-label="Toggle navigation">
        <span class='fas fa-bars fa-lg navToggle'></span>
      </button>
      <div class='container-fluid row row-12'>

        <div class='collapse navbar-collapse' id='navbar'>
          <span id=''>Ellerup Landscaping Logo</span>
          <ul class='navbar-nav ml-auto'>
            <li class='nav-item nav-link'>
              <router-link :to="{ name: 'Home', params: {} }" class='nav-link' exact>
                Home
              </router-link>
            </li>
            <li class='nav-item nav-link'>
              <router-link :to="{ name: 'About', params: {} }" class='nav-link' exact>
                About
              </router-link>
            </li>
            <li class='nav-item nav-link'>
              <router-link to="/contact" class='nav-link' exact>
                Contact
              </router-link>
            </li>
          </ul>
        </div>
        <!-- Close navbar collapse div-->
      </div>
      <!--Close container 1 -->
    </nav>
    <!-- End Nav -->
    <nav>
      <ul>

      </ul>
    </nav>
  </header>
</template>

<script>
export default {
}
</script>

<style lang="scss" scoped>
$primaryColor: #01792a;
$secondaryColor: #39da73;
$accentColor: #3e824f;
$highlightColor: rgb(237, 236, 245);
$linkColor: rgb(37, 150, 153);
$linkHoverColor: $secondaryColor;
$linkActiveColor: $accentColor;
nav {
    background-color: $primaryColor;
    color: white;
    font-family: 'Lato', sans-serif;
    //  border-top: 40px solid $secondaryColor;
    //  border-bottom: 40px solid $primaryColor;
    .navToggle {
        color: white;
    }

    a {
        color: $highlightColor;
    }
    a:hover {
        color: $linkHoverColor;
    }
    a:active {
        color: $linkActiveColor;
    }
    a:focus {
        color: $linkActiveColor;
        background-color: white;
    }
}
.router-link-active {
    color: white;
}
</style>
