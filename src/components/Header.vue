<template>
    <header>
    <div class="aa-header">
      <nav class="navbar navbar-expand-md navbar-transparent">
        <div class="container">
          <img
            class="img-fluid pr-3 aa-logo-img"
            :src="siteLogo"
            :alt="logo"
          /><a class="navbar-brand px-0 py-0" href="#">Awesome App</a>
          <div class="collapse navbar-collapse">
            <ul class="navbar-nav ml-auto">
              <li class="nav-item"><a class="nav-link" href="#">Home</a></li>
              <li class="nav-item">
                <a class="nav-link" href="#features">Features</a>
              </li>
              <li class="nav-item">
                <a class="nav-link" href="#pricing">Pricing</a>
              </li>
              <li class="nav-item">
                <a class="btn btn-outline-neutral btn-round" href="#download"
                  >Download Now</a
                >
              </li>
            </ul>
          </div>
        </div>
      </nav>
      <div class="container aa-header-content text-left text-white">
        <div class="row">
          <div class="col-md-6 col-sm-12">
            <h1 class="text-white mb-4">
               {{ titleOne }}<br />{{ titleTwo }}
            </h1>
            <p>
              {{ text }}
            </p>
            <ul class="py-1 list-unstyled">
              <li class="py-2" v-for="list in lists" :key="list.index">
                <i class="fa fa-check-circle pr-4" aria-hidden="true"></i>
                {{ list }}
              </li>              
            </ul>
            <a class="mt-4 btn btn-outline-neutral btn-round" href="#features"
              >{{ button }}</a
            >
          </div>
          <div class="col-md-6 col-sm-12 text-right">
            <img class="img-fluid" :src="image.img" :alt="image.alt" />
          </div>
        </div>
      </div>
    </div>
  </header>
</template>

<script setup>
const siteLogo = "./../../images/logo.png"
const titleOne = "Awesome App"
const titleTwo = "App Landing Template"
const text = "An awesome landing page template to showcase your app features, screenshots, pricing, user testimonials and download links."
const lists = [
  "Amazing Design to Present Your App ", " Fully Responsive and Powered by Bootstrap & PaperKit", "Very Easy to Customize and Setup "
]
const button = "Start Exploring"
const image = {
  img: "./../../images/1.jpg",
  alt: "Image"
}

</script>