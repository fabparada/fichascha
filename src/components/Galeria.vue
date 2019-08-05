<template>
  <div class="galeria container mt-4">
    <image-list src="image-list" :images="images"></image-list>
  </div>
</template>

<script>
import ImageList from './ImageList'

export default {
  name: 'galeria',
  components: {ImageList},
  data () {
    return {
      selectedImage: '',
      images: [
        {id: 1, title: 'Primera imagen', description: 'desc. prim. img', thumbnail: 'https://videotutoriales.com/egipto01.png', imageLink: 'https://videotutoriales.com/egipto01.png'},
        {id: 2, title: 'segunda imagen', description: 'desc. s. img', thumbnail: 'https://videotutoriales.com/egipto02.png', imageLink: 'https://videotutoriales.com/egipto02.png'},
        {id: 3, title: 'tercera imagen', description: 'desc. t. img', thumbnail: 'https://videotutoriales.com/egipto03.png', imageLink: 'https://videotutoriales.com/egipto03.png'},
        {id: 4, title: 'cuarta imagen', description: 'desc. c. img', thumbnail: 'https://videotutoriales.com/egipto04.png', imageLink: 'https://videotutoriales.com/egipto04.png'},
        {id: 5, title: 'quinta imagen', description: 'desc. q. img', thumbnail: 'https://videotutoriales.com/egipto05.png', imageLink: 'https://videotutoriales.com/egipto05.png'},
        {id: 6, title: 'sexta imagen', description: 'desc. sx. img', thumbnail: 'https://videotutoriales.com/egipto06.png', imageLink: 'https://videotutoriales.com/egipto06.png'},
        {id: 7, title: 'septima imagen', description: 'desc. sp. img', thumbnail: 'https://videotutoriales.com/egipto07.png', imageLink: 'https://videotutoriales.com/egipto07.png'},
        {id: 8, title: 'octava imagen', description: 'desc. oc. img', thumbnail: 'https://videotutoriales.com/egipto08.png', imageLink: 'https://videotutoriales.com/egipto08.png'}

      ]
    }
  },
  methods: {
    showImage: function (image) {
      this.selectedImage = image
    }
  }
}
</script>
