<template>
  <div>
    <div class="px-1 px-sm-3">
      <b-jumbotron class="col-10 mx-auto mt-5 mb-4">
        <template slot="header">
          Powering Innovation.
        </template>
        <template slot="lead">
          Pay-as-you-go development services.<br />
          On-demand, first-class developers.<br />
          Fully-managed agile delivery process.<br />
          Scalable and flexible.<br />
          No contracts and no hassle.
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
        <h4 slot="header" class="mb-0">What We Do</h4>
        <b-card-text>
          We take the pain out of building technology and technology teams. We
          provide on-demand development services utilizing our proprietary
          DevCycles agile methodology to rapidly deliver value to our partners.
        </b-card-text>
        <b-button slot="footer" to="/what-we-do" variant="primary">
          Learn More
        </b-button>
      </b-card>
      <b-card class="my-2">
        <h4 slot="header" class="mb-0">How It Works</h4>
        <b-card-text>
          Header and footers using slots.
        </b-card-text>
        <b-button slot="footer" to="/how-it-works" variant="primary">
          Learn More
        </b-button>
      </b-card>
      <b-card class="my-2" title="Use Cases">
        <h4 slot="header" class="mb-0">Use Cases</h4>
        <b-card-text>
          Header and footers using slots.
        </b-card-text>
        <b-button slot="footer" to="/use-cases" variant="primary">
          Learn More
        </b-button>
      </b-card>
    </b-card-group>
    <div class="text-center mx-auto p-5">
      <b-button to="/pricing" class="p-5">
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
      <b-button variant="primary" to="#" class="p-5">
        Apply Now to Join Our Beta Program
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
