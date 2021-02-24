<template>
  <div id="app">
    <nav class="navbar navbar-expand-lg navbar-light bg-light">
      <!-- Container wrapper -->
      <div class="container-fluid">
        <!-- Toggle button -->
        <button
          class="navbar-toggler"
          type="button"
          data-mdb-toggle="collapse"
          data-mdb-target="#navbarLeftAlignExample"
          aria-controls="navbarLeftAlignExample"
          aria-expanded="false"
          aria-label="Toggle navigation"
        >
          <i class="fas fa-bars"></i>
        </button>

        <!-- Collapsible wrapper -->
        <div class="collapse navbar-collapse" id="navbarLeftAlignExample">
          <!-- Left links -->
          <ul class="navbar-nav me-auto mb-2 mb-lg-0">
            <li class="nav-item">
              <router-link class="nav-link active" to="/">Home</router-link>
            </li>
            <li class="nav-item">
              <router-link class="nav-link active" to="/about">
                About
              </router-link>
            </li>
            <li class="nav-item">
              <router-link class="nav-link active" to="/contact">
                Contact
              </router-link>
            </li>
            <!-- Navbar dropdown -->
            <li class="nav-item dropdown">
              <a
                class="nav-link dropdown-toggle"
                href="#"
                id="navbarDropdown"
                role="button"
                data-mdb-toggle="dropdown"
                aria-expanded="false"
              >
                @MusicStore
              </a>
              <!-- Dropdown menu -->
              <ul class="dropdown-menu" aria-labelledby="navbarDropdown">
                <li>
                  <router-link class="dropdown-item" href="#"
                    >Action</router-link
                  >
                </li>
                <li>
                  <router-link class="dropdown-item" href="#"
                    >Action</router-link
                  >
                </li>
                <li><hr class="dropdown-divider" /></li>
                <li>
                  <router-link class="dropdown-item" href="#"
                    >Action</router-link
                  >
                </li>
              </ul>
            </li>
            <li class="nav-item">
              <a
                class="nav-link disabled"
                href="#"
                tabindex="-1"
                aria-disabled="true"
                >Disabled</a
              >
            </li>
          </ul>
          <!-- Left links -->
        </div>
        <!-- Collapsible wrapper -->
      </div>
      <!-- Container wrapper -->
    </nav>
    <img src="./assets/logo-mdb-vue-small.png" />
    <router-view />
  </div>
</template>

<script lang="javascript">
import * as mdb from 'mdb-ui-kit';

export default {
  name: "App",
  mdb
};
</script>

<style>
@import "~mdb-ui-kit/css/mdb.min.css";
@import url("https://fonts.googleapis.com/css?family=Roboto:300,400,500,700&display=swap");

#app {
  text-align: center;
  margin-top: 150px;
}
</style>
