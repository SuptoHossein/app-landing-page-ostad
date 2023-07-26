<template>
  <div class="aa-price-package section" id="pricing">
    <div class="container">
      <div class="text-center">
        <h2 class="title">{{ title }}</h2>
        <p class="pb-5">
          {{ text }}
        </p>
      </div>
      <div class="row">
        <div class="col-lg-3 col-md-6" v-for="price in prices" :key="price.key">
          <div class="card aa-price text-center">
            <div class="card-body">
              <div class="h5 mt-0">{{ price.title }}</div>
              <div class="aa-price-section" :class="price.isActive ? 'bg-gradient text-white' : ''">
                <sup>$</sup><span>{{ price.price }}</span><small>/m</small>
              </div>
              <ul class="list-unstyled text-muted">
                <li class="pt-3" v-for="feature in price.features" :key="feature.index">
                  {{ feature }}
                </li>
              </ul>
            </div>
            <div class="card-footer">
              <p>
                <a href="#" class="text-muted text-small">{{ link }}</a>
              </p>
              <a class="btn btn-round" :class="price.isActive ? 'bg-gradient' : 'btn-outline-default border'" href="#">{{ buy }}</a>
            </div>
          </div>
        </div>

       
      </div>
    </div>
  </div>
</template>

<script setup>
const title = "We've got the perfect package for you"
const text = "A section to display your pricing structure. Make sure to highlight your most popular plan like shown below.<br />Replace this text to describe your pricing plan."
const link = "Start Free Trial"
const buy = "Buy Now"

const prices = [
  {
    title: "Basic",
    price: "12.0",
    isActive: false,
    features:
      ["One User", "Multiple Access", "SMS Support", "24/7 Online Support"]
  },
  {
    title: "Standard",
    price: "24.0",
    isActive: true,
    features:
      ["Five User", "Multiple Access", "SMS Support", "24/7 Online Support"]
  },
  {
    title: "Premium",
    price: "250.0",
    isActive: false,
    features:
      ["Twenty User", "Multiple Access", "SMS Support", "24/7 Online Support"]
  },
  {
    title: "Enterprise",
    price: "999.0",
    isActive: false,
    features:
      ["One User", "Multiple Access", "SMS Support", "24/7 Online Support"]
  },
]

const features = [
  {
    user: "Unlimited User", access: "Multiple Access", sms: "SMS Support", support: "24/7 Online Support"
  }
]
</script>
