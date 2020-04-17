<template>
  <navbar
    position="fixed"
    type="primary"
    :transparent="transparent"
    :color-on-scroll="colorOnScroll"
    menu-classes="ml-auto"
  >
    <template slot-scope="{ toggle, isToggled }">
      <router-link v-popover:popover1 class="navbar-brand" to="/">
        Tosin's Portfolio
      </router-link>
      <el-popover
        ref="popover1"
        popper-class="popover"
        placement="bottom"
        width="200"
        trigger="hover"
      >
        <div class="popover-body">
          Designed by Tosin Ogunfowote
        </div>
      </el-popover>
    </template>
    <template slot="navbar-menu">
      <li class="nav-item">
        <a
          class="nav-link"
          href="#aboutme"
        >
          <i class="now-ui-icons users_single-02"></i>
          <p>About Me</p>
        </a>
      </li>
      <li class="nav-item">
        <a
          class="nav-link"
          href="#skills"
        >
          <i class="now-ui-icons tech_laptop"></i>
          <p>Skills</p>
        </a>
      </li>
      <li class="nav-item">
        <a
          class="nav-link"
          href="#portfolio"
        >
          <i class="now-ui-icons design_app"></i>
          <p>Portfolio</p>
        </a>
      </li>
      <li class="nav-item">
        <a
          class="nav-link btn btn-neutral"
          href=""
        >
          <i class="now-ui-icons arrows-1_cloud-download-93"></i>
          <p>Download Resume</p>
        </a>
      </li>

      <li class="nav-item">
        <a
          class="nav-link"
          rel="tooltip"
          title="Check me on Git"
          data-placement="bottom"
          href="https://github.com/tofmat"
          target="_blank"
        >
          <i class="fab fa-github"></i>
          <p class="d-lg-none d-xl-none">GitHub</p>
        </a>
      </li>
      <li class="nav-item">
        <a
          class="nav-link"
          rel="tooltip"
          title="Check me on LinkedIn"
          data-placement="bottom"
          href="https://linkedin.com/in/ogunfowotetosin"
          target="_blank"
        >
          <i class="fab fa-linkedin"></i>
          <p class="d-lg-none d-xl-none">LinkedIn</p>
        </a>
      </li>
      <li class="nav-item">
        <a
          class="nav-link"
          rel="tooltip"
          title="Follow us on Twitter"
          data-placement="bottom"
          href="https://www.twitter.com/dtofmat"
          target="_blank"
        >
          <i class="fab fa-twitter"></i>
          <p class="d-lg-none d-xl-none">Twitter</p>
        </a>
      </li>
    </template>
  </navbar>
</template>

<script>
import { DropDown, NavbarToggleButton, Navbar, NavLink } from '@/components';
import { Popover } from 'element-ui';
export default {
  name: 'main-navbar',
  props: {
    transparent: Boolean,
    colorOnScroll: Number
  },
  components: {
    DropDown,
    Navbar,
    NavbarToggleButton,
    NavLink,
    [Popover.name]: Popover
  }
};
</script>

<style scoped></style>
