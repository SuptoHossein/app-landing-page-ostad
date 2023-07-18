<template>
  <div class="aa-download-section section bg-gradient" id="download">
    <div class="container">
      <div class="h2 text-center text-title text-white pb-5">
        {{ title }}
      </div>
      <div class="row">
        <div class="col-md-4 col-sm-12">
          <a class="aa-apple" href="#">
            <div class="card">
              <div class="row pb-3">
                <div class="col-lg-3 col-md-12 aa-download-icon">
                  <i class="pt-4 fa fa-apple fa-4x" aria-hidden="true"></i>
                </div>
                <div class="col-lg-9 col-md-12 aa-download-icon-detail">
                  <div class="h4 pb-1">{{ apple.title }}</div>
                  <p class="text-muted">{{ apple.text }}</p>
                </div>
              </div>
            </div>
          </a>
        </div>
        <div class="col-md-4 col-sm-12">
          <a class="aa-android" href="#">
            <div class="card">
              <div class="row pb-3">
                <div class="col-lg-3 col-md-12 aa-download-icon">
                  <i class="pt-4 fa fa-android fa-4x" aria-hidden="true"></i>
                </div>
                <div class="col-lg-9 col-md-12 aa-download-icon-detail">
                  <div class="h4 pb-1">{{ android.title }}</div>
                  <p class="text-muted">{{ android.text }}</p>
                </div>
              </div>
            </div>
          </a>
        </div>
        <div class="col-md-4 col-sm-12">
          <a class="aa-windows" href="#">
            <div class="card">
              <div class="row pb-3">
                <div class="col-lg-3 col-md-12 aa-download-icon">
                  <i class="pt-4 fa fa-windows fa-4x" aria-hidden="true"></i>
                </div>
                <div class="col-lg-9 col-md-12 aa-download-icon-detail">
                  <div class="h4 pb-1">{{ microsoft.title }}</div>
                  <p class="text-muted">{{ microsoft.text }}</p>
                </div>
              </div>
            </div>
          </a>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
const title = "Download Awesome App Now"

const apple = {
  title: "Download",
  text: "Download from App Store"
}
const android = {
  title: "Download",
  text: "Download from Play Store"
}
const microsoft = {
  title: "Download",
  text: "Download from Microsoft Store"
}

</script>