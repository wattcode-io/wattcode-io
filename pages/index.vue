<template>
  <div>
    <div class="px-1 px-sm-3">
      <b-jumbotron class="col-10 mx-auto mt-5 mb-4">
        <template slot="header">
          Powering Innovation.
        </template>
        <template slot="lead">
          On-demand software development services.<br />
          First-class developers.<br />
          Fully-managed agile delivery process.<br />
          Scalable and flexible.<br />
          Pay-as-you-go, no contracts and no hassle.
        </template>
        <hr class="my-4" />
        <p>
          We're currently running a private beta program for select customers.
          <br />
          Contact us to apply.
        </p>
        <b-button variant="primary" class="mt-2" to="#">Get Started</b-button>
      </b-jumbotron>
    </div>
    <b-card-group deck class="col-10 px-0 mx-auto my-3">
      <!-- <b-card
        title="What We Do"
        img-src="/developer-coding-on-laptop_4460x4460-e1542890619241.jpg"
        img-alt="Software Developer at Computer"
        img-top
      >
        <h6 slot="header" class="mb-0">Header Slot</h6>
        <b-card-text>We provide on-demand software development</b-card-text>
        <b-button to="/what-we-do" variant="primary">Learn More</b-button>
      </b-card> -->
      <b-card class="my-4">
        <h4 slot="header" class="mb-0 px-3">What We Do</h4>
        <b-card-text class="px-3">
          Wattcode provides fully-managed, on-demand software development
          services. We provide the people and process to build the technology
          needed to power your business. Our teams can be innovating for you
          within 24 hours!
        </b-card-text>
        <b-button slot="footer" to="/what-we-do" variant="primary" class="ml-3">
          Services
        </b-button>
      </b-card>
      <b-card class="my-4">
        <h4 slot="header" class="mb-0 px-3">How It Works</h4>
        <b-card-text class="px-3">
          We utilize our proprietary PowerCycles agile methodology and flexible
          application templates to rapidly deliver value. Our delivery
          management team works with you to handle planning and execution,
          resulting in the hassle-free development of quality custom software.
        </b-card-text>
        <b-button
          slot="footer"
          to="/how-it-works"
          variant="primary"
          class="ml=3"
        >
          Benefits
        </b-button>
      </b-card>
      <b-card class="my-4">
        <h4 slot="header" class="mb-0 px-3">What It Costs</h4>
        <b-card-text class="px-3">
          Wattcode offers a unique, no-contract, pay-as-you-go model. Engage a
          single-developer to supplement your team, or entire squads to deliver
          larger projects. Flex your team as required to meet your business
          goals. Our model is designed to maximize the value delivered.
          <!-- - no daily or weekly rates where you
          are paying to cover internal meeting time, long meal breaks or
          personal time off. -->
        </b-card-text>
        <b-button slot="footer" to="/use-cases" variant="primary">
          Pricing
        </b-button>
      </b-card>
    </b-card-group>
    <!-- <div class="text-center py-5 use-cases">
      <div>
        <h3>Use Cases</h3>
      </div>
      <b-button
        to="/use-cases"
        class="col-8 col-sm-6 col-lg-3 col-xl-2 mx-4 my-4 py-4"
      >
        Startups
      </b-button>
      <b-button class="col-8 col-sm-6 col-lg-3 col-xl-2 mx-4 my-4 py-4">
        Agencies
      </b-button>
      <b-button class="col-8 col-sm-6 col-lg-3 col-xl-2 mx-4 my-4 py-4">
        Transformation
      </b-button>
    </div> -->
    <hr class="col-12" />
    <div class="text-center mx-auto px-2 pt-5">
      <h3>Testimonials</h3>
    </div>
    <b-carousel
      id="carousel-fade"
      style="text-shadow: 0px 0px 2px #000; width: 30%"
      class="mx-auto mt-3 mb-3"
      :interval="0"
      fade
    >
      <b-carousel-slide
        img-src="/real-vision.png"
        class="d-block img-fluid w-100"
      >
      </b-carousel-slide>
    </b-carousel>
    <div class="text-center mx-auto px-2 mb-5">
      <i class="mt-5">
        "Wattcode is like AWS for software development services."
      </i>
      <br />
      <span>-- Bofei Cao, CEO</span>
    </div>
    <hr class="col-12" />
    <div class="text-center mx-auto p-5">
      <b-button
        variant="primary"
        to="#"
        class="col-10 col-sm-9 col-md-7 col-lg-5 col-xl-4 p-5"
      >
        Apply to Join Our Beta Program
      </b-button>
    </div>
  </div>
</template>

<style lang="scss" scoped>
@import '../assets/wattcode.scss';

// number of cards per line for each breakpoint
$cards-per-line: (
  xs: 1,
  sm: 1,
  md: 1,
  lg: 3,
  xl: 3
);

@each $name, $breakpoint in $grid-breakpoints {
  @media (min-width: $breakpoint) {
    .card-deck .card {
      flex: 0 0
        calc(#{100 / map-get($cards-per-line, $name)}% - #{$grid-gutter-width});
    }
  }
}

.use-cases {
  border-top: 1px solid $gray-400;
  border-bottom: 1px solid $gray-400;
  background-color: $gray-100;
}
</style>
