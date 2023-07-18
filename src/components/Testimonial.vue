<template>
  <div class="aa-testimonials-section section">
    <div class="container">
      <div class="text-center">
        <h2 class="title mt-0">{{ title }}</h2>
        <p>
          {{ text }}
        </p>
      </div>
      <div class="aa-testimonials">
        <div class="row">
          <div class="col-md-4 mb-3" v-for="testimonial in testimonials" :key="testimonial.index">
            <div class="aa-testimonials-body">
              <p>
                {{ testimonial.text }}
              </p>
              <div class="row pt-3">
                <div class="col-lg-5 col-md-12">
                  <img class="img-fluid" :src="testimonial.image" alt="Face 1" />
                </div>
                <div class="col-lg-7 col-md-12 pt-3">
                  <div class="h5">{{ testimonial.name }}</div>
                  <p class="text-muted">{{ testimonial.designation }}</p>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
const title = "What our customers are saying"
const text = `Real user testimonials are great way to attract new customers and increase their trust into using your app. Replace the testimonials below with the ones for your own app.`

const testimonials = [
  {
    text: `Awesome App is awesome and I can't imagine working on my projects without it. It has saved me countless hours of time and has increased my productivity.`,
    name: "Patrick Harry",
    designation: "CEO, Awesome Inc.",
    image: "./../src/assets/images/user1.jpg",
    alt: "Face 1"
  },
  {
    text: `Awesome App is awesome and I can't imagine working on my projects without it. It has saved me countless hours of time and has increased my productivity.`,
    name: "Jeanne Lawson",
    designation: "Design, Awesome Inc",
    image: "./../src/assets/images/user2.jpg",
    alt: "Face 2"
  },
  {
    text: `Awesome App is awesome and I can't imagine working on my projects without it. It has saved me countless hours of time and has increased my productivity.`,
    name: "Robin Barnes",
    designation: "Developer, Awesome Inc",
    image: "./../src/assets/images/user3.jpg",
    alt: "Face 3"
  },
]
</script>