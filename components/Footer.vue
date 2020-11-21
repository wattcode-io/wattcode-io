<template>
  <b-container fluid class="footerContainer mt-4 pb-5">
    <b-row align-h="around">
      <b-col cols="8" sm="8" md="3" lg="3" xl="2" class="pt-4">
        <h5>Work at Wattcode</h5>
        <b-nav vertical>
          <b-nav-item to="/work/how-we-work">
            How We Work
          </b-nav-item>
          <b-nav-item to="/work/available-positions">
            Available Positions
          </b-nav-item>
        </b-nav>
      </b-col>
      <b-col cols="8" sm="8" md="2" lg="1" xl="1" class="pt-4">
        <h5>About</h5>
        <b-nav vertical>
          <!-- <b-nav-item to="/blog">Blog</b-nav-item> -->
          <b-nav-item to="/contact">Contact</b-nav-item>
          <!-- <b-nav-item to="/privacy">Privacy</b-nav-item>
          <b-nav-item to="/legal">Legal</b-nav-item> -->
        </b-nav>
      </b-col>
    </b-row>
  </b-container>
</template>

<style lang="scss" scoped>
@import '../assets/wattcode.scss';

.footerContainer {
  border-top: 1px solid $gray-400;
  background-color: $gray-200;
}

.nav-link {
  padding: 0.25rem 0;
  color: theme-color(dark);
}

a:hover {
  color: black;
}
</style>
