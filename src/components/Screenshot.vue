<template>
  <div class="aa-screenshots section">
    <div class="container text-center">
      <h2 class="title pb-3">{{ screenshotData.title }}</h2>
      <p class="pb-5">
        {{ screenshotData.text }}
      </p>
      <div class="row">
        <div class="col-md-12 mb-5">
          <div class="card card-raised page-carousel">
            <div
              class="carousel slide"
              id="aa-carousel-indicators"
              data-ride="carousel"
            >
              <ol class="carousel-indicators">
                <li
                  class="active"
                  data-target="#aa-carousel-indicators"
                  data-slide-to="0"
                ></li>
                <li
                  class=" "
                  data-target="#aa-carousel-indicators"
                  data-slide-to="1"
                ></li>
                <li
                  class=" "
                  data-target="#aa-carousel-indicators"
                  data-slide-to="2"
                ></li>
              </ol>
              <div class="carousel-inner" role="listbox">
                <div class="carousel-item" v-for="slide in slides" :key="slide.index">
                  <img
                    class="img-fluid"
                    :src="slide.image"
                    :alt="slide.alt"
                  />
                  <div class="carousel-caption d-none d-md-block"></div>
                </div>                
              </div>
              <a
                class="left carousel-control carousel-control-prev bg-danger"
                href="#aa-carousel-indicators"
                role="button"
                data-slide="prev"
                ><span class="fa fa-angle-left"></span
                ><span class="sr-only">Previous</span></a
              ><a
                class="right carousel-control carousel-control-next bg-danger"
                href="#aa-carousel-indicators"
                role="button"
                data-slide="next"
                ><span class="fa fa-angle-right"></span
                ><span class="sr-only">Next</span></a
              >
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
const screenshotData = {
  title: "Take a look at our screenshots",
  text: `Add your app screenshots below. Make sure to make them lively by putting them inside real device mockups \n Replace this text to describe the screenshots of your app.`,
};

const slides = [
    { image: "./src/assets/images/3.jpg", alt: "First slide"},
    { image: "./src/assets/images/4.jpg", alt: "Second slide"},
    { image: "./src/assets/images/5.jpg", alt: "Third slide"},
]
</script>