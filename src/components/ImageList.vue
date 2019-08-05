<template>
  <div class="galeria container mt-4">
    <div class="row">
        <div class= "col-sm-8 col-12" >
            <img :src="selectedImage.imageLink" class="img-fluid">
        </div>
        <div class="col-sm-4 col-12">
          <h1>{{ selectedImage.title }}</h1>
          <p>{{ selectedImage.description }}</p>
        </div>
    </div>
    <div class="row" >
      <div v-for="image in images" :key="image.id" class="col-md-3 col-sm-4 col-6"><a href="#" v-on:click="showImage(image)"><img class="img-fluid" v-bind:src="image.thumbnail"/></a></div>
    </div>
</div>
</template>

<script>
export default {
  props: ['images'],
  data () {
    return {
        selectedImage: '',
      }
    },
    methods: {
        showImage: function (image) {
          this.selectedImage = image
        }
      }
    }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
img {
  -webkit-box-shadow: 0px 1px 6px 1px rgba(0,0,0,0.2);
  -moz-box-shadow: 0px 1px 6px 1px rgba(0,0,0,0.2);
  box-shadow: 0px 1px 6px 1px rgba(0,0,0,0.2);
  margin-bottom:20px;
}
img:hover {
  filter: gray;
  -webkit-filter: grayscale(1);
}
</style>
