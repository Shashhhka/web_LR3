<script setup>
const events = [
  {
    img: {
      src: '../../img/dragon.svg',
      alt: 'dragon'
    },
    description: 'Chinese New Year'
  },
  {
    img: {
      src: '../../img/valentine.svg',
      alt: 'valentine'
    },
    description: 'The Night of Sevens'
  },
    {
    img: {
      src: '../../img/branch.svg',
      alt: 'branch'
    },
    description: 'Peach blossom'
  },
    {
    img: {
      src: '../../img/butterfly.svg',
      alt: 'butterfly'
    },
    description: 'Butterfly festival'
  },
    {
    img: {
      src: '../../img/chinese_lantern.svg',
      alt: 'chinese_lantern'
    },
    description: 'Ghost City festival'
  },
    {
    img: {
      src: '../../img/rabbit.svg',
      alt: 'rabbit'
    },
    description: 'Mid-autumn festival'
  },
]
</script>

<template>
  <div class="container">
    <div class="events">
      <h2>Events</h2>
      <hr>

      <div class="catalog">
        <div class="row">
          <div class="col-md-6 col-lg-4"
               v-for="(item, index) in events"
               :key="index">
            <div class="catalog__item">
              <img :src="item.img.src" :alt="item.alt" class="catalog__img">
              <div class="catalog__vertical-line">
                <p class="catalog__text">{{item.description}}</p>
                <span class="arrow">
                    <span></span>
                </span>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>

    <div class="tickets">
      <h2>GET THE LATEST NEWS<br>ABOUT OUR EVENTS</h2>
      <p class="tickets__subtitle">Just register to our newsletter and don’t miss anything<br>anymore. We promise
        not to spam you!</p>
      <div class="d-flex justify-content-center">
        <div class="input-group">
          <input type="text" class="form-control" placeholder="Enter your e-mail"
                 aria-label="Enter your e-mail" aria-describedby="inp">
          <span class="input-group-text" id="inp">Subscribe</span>
        </div>
      </div>

    </div>
  </div>
</template>

<style scoped>

</style>