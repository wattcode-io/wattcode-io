<template>
  <div>
    <div class="px-1 px-sm-3">
      <b-jumbotron class="col-10 mx-auto mt-5 mb-4">
        <template slot="header">
          Powering Innovation.
        </template>
        <template slot="lead">
          On-demand development services.<br />
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
    <b-card-group deck class="col-10 px-0 mx-auto">
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
      <b-card class="my-2">
        <h4 slot="header" class="mb-0 px-3">What We Do</h4>
        <b-card-text class="px-3">
          Wattcode builds software to power your business. We provide
          cloud-based, on-demand software development services, utilizing our
          proprietary PowerCycles agile methodology to rapidly deliver value to
          our partners. Our on-demand services can be engaged and contributing
          to your projects in as little as 24-hours.
        </b-card-text>
        <b-button slot="footer" to="/what-we-do" variant="primary" class="ml-3">
          Learn More
        </b-button>
      </b-card>
      <b-card class="my-2">
        <h4 slot="header" class="mb-0 px-3">How It Works</h4>
        <b-card-text class="px-3">
          Wattcode makes it easy to scale development teams. With our flexible
          model, you can engage a single-developer to supplement your team, or
          entire squads to deliver larger projects. Our delivery team partners
          with you to understand and prioritize work, and handles all
          coordination with our vetted, first-class development resources to
          deliver high-quality software.
        </b-card-text>
        <b-button
          slot="footer"
          to="/how-it-works"
          variant="primary"
          class="ml=3"
        >
          Learn More
        </b-button>
      </b-card>
      <b-card class="my-2">
        <h4 slot="header" class="mb-0 px-3">Use Cases</h4>
        <b-card-text class="px-3">
          Wattcode helps accelerate software projects. Speed time to market by
          engaging Wattcode squads rather than wait for internal teams to be
          hired and on-boarded. Add capacity to take on that unexpected new
          client with Wattcode resources. Bring in specialized expertize to
          drive innovation. Wattcode delivers the software projects you need,
          when you need them.
        </b-card-text>
        <b-button slot="footer" to="/use-cases" variant="primary">
          Learn More
        </b-button>
      </b-card>
    </b-card-group>
    <div class="text-center mx-auto p-5">
      <b-button to="/pricing" class="col-10 col-sm-8 col-lg-6 p-5">
        View Availability and Pricing
      </b-button>
    </div>
    <div class="text-center mx-auto p-2">
      <h3>See Our Customer Stories</h3>
    </div>
    <b-carousel
      id="carousel-fade"
      style="text-shadow: 0px 0px 2px #000; width: 40%"
      class="mx-auto"
      :interval="0"
      fade
    >
      <b-carousel-slide
        img-src="/real-vision.png"
        class="d-block img-fluid w-100"
      ></b-carousel-slide>
    </b-carousel>
    <div class="text-center mx-auto p-5">
      <b-button variant="primary" to="#" class="col-10 col-sm-8 col-lg-6 p-5">
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
</style>
