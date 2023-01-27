<template>
  <main>

  <section class="py-5 text-center container">
    <div class="row py-lg-5">
      <div class="col-lg-6 col-md-8 mx-auto">
        <h1 class="fw-light">Album example</h1>
        <p class="lead text-muted">Something short and leading about the collection below—its contents, the creator, etc. Make it short and sweet, but not too short so folks don’t simply skip over it entirely.</p>
        <p>
          <a href="#" class="btn btn-primary my-2">Main call to action</a>
          <a href="#" class="btn btn-secondary my-2">Secondary action</a>
        </p>
      </div>
    </div>
  </section>

  <div class="album py-5 bg-light">
    <div class="container">

      <div class="row row-cols-1 row-cols-sm-2 row-cols-md-3 g-3">

        <!--<template v-for="i in items" :key="i">        
          <AlbumItem />
        </template>   -->

        <template v-for="i in items" :key="i">
          <AlbumItemVideo />
        </template>     
      

       
        
       
      </div>
    </div>
  </div>

</main>
</template>

<script>
/* eslint-disable */
import AlbumItem from '@/components/AlbumItem.vue'
import AlbumItemVideo from '@/components/AlbumItemVideo.vue'
export default {
  components: { AlbumItem, AlbumItemVideo },
  name: "MyMain",
  data(){
    return {
      items: [1,2,3,4,5,6,7,8,9]
    }
  }
}
</script>

<style>

</style>