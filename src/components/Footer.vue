<template>
    <footer class="footer-black aa-footer">
    <div class="container py-5">
      <div class="row text-center">
        <div class="col-md-12">
          <a class="btn btn-link btn-neutral" href="#"
            ><i class="fa fa-facebook fa-2x" aria-hidden="true"></i></a
          ><a class="btn btn-link btn-neutral" href="#"
            ><i class="fa fa-twitter fa-2x" aria-hidden="true"></i></a
          ><a class="btn btn-link btn-neutral" href="#"
            ><i class="fa fa-google-plus fa-2x" aria-hidden="true"></i></a
          ><a class="btn btn-link btn-neutral" href="#"
            ><i class="fa fa-instagram fa-2x" aria-hidden="true"></i
          ></a>
        </div>
        <div class="col-md-12">
          <p class="mt-3">
            {{ titleOne }}<br />{{ titleTwo }}
            <a class="credit" href="https://templateflip.com" target="_blank"
              >{{ link }}</a
            >
          </p>
        </div>
      </div>
    </div>
  </footer>
</template>

<script setup>
const titleOne = "Copyright &copy; Awesome App. All rights reserved."
const titleTwo = "Design -"
const link = "TemplateFlip"
</script>