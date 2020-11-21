<template>
  <div>
    <h1>Wattcode Pricing</h1>
    <p>
      Wattcode offers a pay-as-you-go pricing model for our cloud-based,
      on-demand development services, allowing you to easily and
      cost-effectively scale your team to match current business needs. With our
      unique DevWatts billing model, you only pay for the effort used for your
      projects. We've eliminated the concept of "daily", "weekly" or "monthly"
      rates, which in many cases means that you're paying for the partner's
      overhead such as their internal meetings, meal breaks and personal time
      off.
    </p>
    <div class="text-center">
      <h3>How Do You Pay for Wattcode Resources</h3>
    </div>
    <b-card-group deck class="col-10 px-0 mx-auto my-3">
      <b-card class="my-4">
        <h4 slot="header" class="mb-0 px-3">DevWatts&trade; Billing</h4>
        <b-card-text class="px-3">
          Our core services are billed based on DevWatts consumed. A DevWatt is
          a small increment of time that a resource spends on your project. For
          typical resources, there are six (6) DevWatts per hour. We bill only
          for time resources spend working on your projects, in a typical 8-hour
          day, a development resource will contribute approximately 35-42
          DevWatts to your projects. This results in an immediate savings of up
          to 25% when compared to an equivalent "daily" rate.
        </b-card-text>
        <b-button slot="footer" to="/what-we-do" variant="primary" class="ml-3">
          Sample Invoice
        </b-button>
      </b-card>
      <b-card class="my-4">
        <h4 slot="header" class="mb-0 px-3">Pay-As-You-Go</h4>
        <b-card-text class="px-3">
          Our flexible, no-commitment model makes it easy to scale development
          teams as needed. Engage a single-developer to supplement your team, or
          entire squads to deliver larger projects. Our delivery management
          services work with you to handle prioritization, planning and project
          management, resulting in the rapid, hassle-free development of
          high-quality software to take your business to new heights.
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
      <b-card class="my-4">
        <h4 slot="header" class="mb-0 px-3">Ways to Save</h4>
        <b-card-text class="px-3">
          Wattcode offers two ways to save even more: Reserved and As-Available
          Resources.<br />
          <strong>Dedicated Resources</strong>
          Use Dedicated Resources to lower your usage rates when you commit to
          longer-term utilization. With Dedicated Resources, you choose between
          a 6-month and 12-month commitment, make a partial up-front payment,
          and then pay a reduced rate for DevWatts utilized each month. The
          exact discount varies by service and commitment length, but for most
          services results in savings of up to 25%.
          <strong>As-Available Resources</strong>
          As-Available Resources take advantage of excess capacity to offer the
          lowest possible rates. Our resources can take on smaller,
          lower-priority items in your backlog as
        </b-card-text>
        <b-button slot="footer" to="/use-cases" variant="primary">
          Learn More
        </b-button>
      </b-card>
    </b-card-group>
  </div>
</template>
