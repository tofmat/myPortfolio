<template>
  <div>
    <div class="page-header clear-filter" filter-color="orange">
      <parallax
        class="page-header-image"
        style="background-image:url('img/bg5.jpg')"
      >
      </parallax>
      <div class="container">
        <div class="photo-container">
          <img src="img/myAvatar.png" alt="" />
        </div>
        <h3 class="title">Tosin Ogunfowote</h3>
        <p class="category">Front End Developer <br/> Project Manager</p>
        <div class="content">
          <div class="social-description">
            <h2>3+ Years</h2>
            <p>Experience</p>
          </div>
          <div class="social-description">
            <h2> > 35</h2>
            <p>Repositories</p>
          </div>
        </div>
      </div>
    </div>
    <div class="section"  id="aboutme">
      <div class="container">
        <div class="button-container">
          <a href="mailto:me@tosinogunfowote.com" v-popover:popover1 class="btn-primary btn btn-round btn-lg">Hire me
            <el-popover
              ref="popover1"
              popper-class="popover"
              placement="bottom"
              width="200"
              trigger="hover"
            >
              <div class="popover-body">
                Shoot me a mail to discuss hiring me.
              </div>
            </el-popover>
          </a>
          
        </div>

    <nucleo-icons-section></nucleo-icons-section>
    <basic-elements id="skills"></basic-elements>

        <div class="row" id="portfolio">
          <div class="col-md-6 ml-auto mr-auto">
            <h4 class="title text-center">My Portfolio</h4>
          </div>
          <tabs
            pills
            class="nav-align-center"
            tab-content-classes="gallery"
            tab-nav-classes="nav-pills-just-icons"
            type="primary"
          >
            <tab-pane title="Profile">
              <i slot="label" class="fab fa-wordpress"></i>

              <div class="col-md-10 ml-auto mr-auto">
                <div class="row collections">
                  <div class="col-md-6">
                    <a href="http://frontiersafrica.org"> <img src="img/w1.png" class="img-raised"/> </a>
                  </div>
                  <div class="col-md-6">
                    <a href="https://saf-ng.org"> <img src="img/w2.png" class="img-raised"/> </a>
                  </div>
                </div>
              </div>
            </tab-pane>

            <tab-pane title="Home">
              <i slot="label" class="fab fa-vuejs"></i>

              <div class="col-md-10 ml-auto mr-auto">
                <div class="row collections">
                  <div class="col-md-6">
                    <img src="img/v1.png" class="img-raised" />
                    <img src="img/v3.png" class="img-raised" />
                  </div>
                  <div class="col-md-6">
                    <img src="img/v2.png" alt="" class="img-raised" />
                    <img src="img/v4.png" alt="" class="img-raised" />
                  </div>
                </div>
              </div>
            </tab-pane>

            <tab-pane title="Messages">
              <i slot="label" class="fas fa-code"></i>

              <div class="col-md-10 ml-auto mr-auto">
                <div class="row collections">
                  <div class="col-md-6">
                    <img src="img/c1.png" class="img-raised" />
                  </div>
                  <div class="col-md-6">
                    <img src="img/c2.png" class="img-raised" />
                  </div>
                </div>
              </div>
            </tab-pane>
          </tabs>
        </div>
      </div>
    <download-section></download-section>

      
    </div>
  </div>
</template>
<script>
import { Tabs, TabPane } from '@/components';
import NucleoIconsSection from './components/NucleoIconsSection';
import BasicElements from './components/BasicElementsSection';
import DownloadSection from './components/DownloadSection';


import { Popover } from 'element-ui';

export default {
  name: 'profile',
  bodyClass: 'profile-page',
  components: {
    Tabs,
    TabPane,
    BasicElements,
    NucleoIconsSection,
    DownloadSection,
    [Popover.name]: Popover
  }
};
</script>
<style>

</style>
