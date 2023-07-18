<template>
  <div class="aa-product-features section">
    <div class="container">
      <div class="row">
        <div class="col-md-5 col-sm-12">
          <img class="img-fluid" :src="imageData.image" :alt="imageData.alt" />
        </div>

        <div class="col-md-7 col-sm-12">
          <h2 class="title mb-2">{{ aboutData.title }}</h2>
          <p class="pt-2">
            {{ aboutData.descOne }}
          </p>
          <p class="pt-5 pb-1">
            {{ aboutData.descTwo }}
          </p>
          <ul class="py-1 list-unstyled">
            <li class="py-1" v-for="list in aboutData.lists" :key="list.index">
              <i class="fa fa-check-circle pr-4" aria-hidden="true"></i>
              {{ list }}
            </li>
          </ul>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
const imageData = {
  image: "./../../images/2.jpg",
  alt: "Image"
}  

const aboutData = {
  title: "What is Awesome App?",
  descOne: "Add a brief story about your app here, what purpose your app solves and why you think your user would want to have it on their device.",
  descTwo: "Re-establish the main use case of your app by listing them below. Make sure to place a relavent screenshot on the left.",
  lists: [
    "Amazing Design to Present Your App", "Fully Responsive and Powered by Bootstrap &amp; PaperKit", "Very Easy to Customize and Setup"
  ]
}


  
</script>