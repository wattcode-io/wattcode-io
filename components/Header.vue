<template>
  <b-container fluid class="headerContainer">
    <b-navbar toggleable="lg" type="dark" class="d-flex flex-row p-2">
      <b-navbar-brand
        to="/"
        class="col-6 col-sm-5 col-md-4 col-lg-3 col-xl-3 p-0"
      >
        <b-img src="/wattcode_logo1.png" class="img-fluid p-2" />
      </b-navbar-brand>

      <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

      <b-collapse id="nav-collapse" is-nav>
        <b-navbar-nav class="mt-1">
          <b-nav-item to="/services" class="align-self-end">
            Services
          </b-nav-item>
          <b-nav-text class="d-none d-lg-block mx-2">|</b-nav-text>
          <b-nav-item to="/benefits" class="align-self-end">
            Benefits
          </b-nav-item>
          <b-nav-text class="d-none d-lg-block mx-2">|</b-nav-text>
          <b-nav-item to="/pricing" class="align-self-end">
            Pricing
          </b-nav-item>
          <!-- <b-nav-text class="d-none d-lg-block mx-2">|</b-nav-text> -->
          <!-- <b-nav-item to="/use-cases" class="align-self-end">
            Use Cases
          </b-nav-item>
          <b-nav-text class="d-none d-lg-block mx-2">|</b-nav-text> -->
          <!-- <b-nav-item to="/resources" class="align-self-end">
            Resources
          </b-nav-item> -->
          <!-- <b-nav-item-dropdown text="Work at Wattcode" class="align-self-end">
            <b-dropdown-item to="/work-at-wattcode/how-we-work">
              How We Work
            </b-dropdown-item>
            <b-dropdown-divider />
            <b-dropdown-item to="/work-at-wattcode/available-positions">
              Available Positions
            </b-dropdown-item>
          </b-nav-item-dropdown> -->
          <b-nav-item
            href="https://wattcode.monday.com"
            target="_blank"
            class="d-block d-lg-none align-self-end"
          >
            Dashboard
          </b-nav-item>
        </b-navbar-nav>
      </b-collapse>
      <b-button
        href="https://wattcode.monday.com"
        target="_blank"
        variant="primary"
        class="d-none d-lg-block mt-1"
      >
        Dashboard
      </b-button>
    </b-navbar>
  </b-container>
  <!-- <b-nav-item-dropdown text="Lang" right>
          <b-dropdown-item href="#">EN</b-dropdown-item>
          <b-dropdown-item href="#">ES</b-dropdown-item>
          <b-dropdown-item href="#">RU</b-dropdown-item>
          <b-dropdown-item href="#">FA</b-dropdown-item>
        </b-nav-item-dropdown> -->
  <!-- <b-container fluid>
    <b-row>
      <b-col>
        <b-img src="/wattcode_logo1.png" class="headerLogo" />
      </b-col>
      <b-col>
        <b-nav>
          <b-nav-item>What We Do</b-nav-item>
          <b-nav-item>How It Works</b-nav-item>
          <b-nav-item>Use Cases</b-nav-item>
          <b-nav-item>Resources &amp; Pricing</b-nav-item>
          <b-nav-item>Work at Wattcode</b-nav-item>
        </b-nav>
      </b-col>
      <b-col cols="1">
        <button>Sign In</button>
      </b-col>
    </b-row>
  </b-container> -->
</template>

<style scoped>
.headerContainer {
  background-color: black;
}
</style>
