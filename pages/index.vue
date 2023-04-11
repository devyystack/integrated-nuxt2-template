<template>
  <div class="content">

<div class="slider">
  <div class="swiper">
    <splide :options="options" style="max-width: 100%;">
      <splide-slide  v-for="(b, i) in banners" :key="i" >
        <div class="picture double" v-if = "b.img != null">
          <img :src="require('@/assets/images/'+  b.img)" style=""/>
        </div>
      </splide-slide>
    </splide>
  </div>
</div>

<div class="news">
  <div class="news-title flex-s-c">
    <span class="news-title_t">News</span>
    <div class="select" tabindex="1">
      <span class="select_value">All News</span>
      <ul class="select_dropdown">
        <li class="select_option">All News</li>
        <li class="select_option">Event</li>
        <li class="select_option">Important</li>
        <li class="select_option">Update</li>
      </ul>
    </div>
  </div>
  <div class="newsBlock">
    <div class="news-block flex-s-c">
      <div class="news-block_l">
        <a href="#">Update 3.14 - “Darkness Rising” is Alive</a>
      </div>
      <div class="news-block_r">
        <span class="color-green">[UPDATE]</span> 01/02/2022
      </div>
    </div>
    <div class="news-block flex-s-c">
      <div class="news-block_l">
        <a href="#">Errors in Farm, Level and Fishery Maps. Errors in Farm, Level and Fishery Maps</a>
      </div>
      <div class="news-block_r">
        <span class="color-red">[IMPORTANT]</span> 01/02/2022
      </div>
    </div>
    <div class="news-block flex-s-c">
      <div class="news-block_l">
        <a href="#">Monster Bash Event</a>
      </div>
      <div class="news-block_r">
        <span class="color-blue">[Event]</span> 01/02/2022
      </div>
    </div>
    <div class="news-block flex-s-c">
      <div class="news-block_l">
        <a href="#">Pets System - New incubators for Bosses</a>
      </div>
      <div class="news-block_r">
        <span class="color-green">[Update]</span> 01/02/2022
      </div>
    </div>
  </div><!--newsBlock-->
</div>

<div class="topHome flex-s">
  <div class="topHome-50">
    <div class="topHome-title flex-s-c">
      <span>TOP Players</span> <a href="" class="button button-small">View More</a>
    </div>
    <table class="top-table">
      <thead>
        <tr>
          <td>#</td>
          <td>Name</td>
          <td>Empire</td>
          <td>Race</td>
          <td>Level</td>
        </tr>
      </thead>
      <tbody>
        <tr>
          <td>1</td>
          <td><a href="">Vex</a></td>
          <td><span class="clan">Shinsso</span></td>
          <td><span class="warrior">Warrior</span></td>
          <td>250</td>
        </tr>
        <tr>
          <td>2</td>
          <td><a href="">Very_Long_Nick_Name</a></td>
          <td><span class="clan">Shinsso</span></td>
          <td><span class="warrior">Warrior</span></td>
          <td>250</td>
        </tr>
        <tr>
          <td>3</td>
          <td><a href="">Vex</a></td>
          <td><span class="clan">Shinsso</span></td>
          <td><span class="warrior">Warrior</span></td>
          <td>250</td>
        </tr>
        <tr>
          <td>4</td>
          <td><a href="">Vex</a></td>
          <td><span class="clan">Shinsso</span></td>
          <td><span class="warrior">Warrior</span></td>
          <td>250</td>
        </tr>
        <tr>
          <td>5</td>
          <td><a href="">Vex</a></td>
          <td><span class="clan">Shinsso</span></td>
          <td><span class="warrior">Warrior</span></td>
          <td>250</td>
        </tr>
        <tr>
          <td>6</td>
          <td><a href="">Vex</a></td>
          <td><span class="clan">Shinsso</span></td>
          <td><span class="warrior">Warrior</span></td>
          <td>250</td>
        </tr>
        <tr>
          <td>7</td>
          <td><a href="">Vex</a></td>
          <td><span class="clan">Shinsso</span></td>
          <td><span class="warrior">Warrior</span></td>
          <td>250</td>
        </tr>
        <tr>
          <td>8</td>
          <td><a href="">Vex</a></td>
          <td><span class="clan">Shinsso</span></td>
          <td><span class="warrior">Warrior</span></td>
          <td>250</td>
        </tr>
        <tr>
          <td>9</td>
          <td><a href="">Vex</a></td>
          <td><span class="clan">Shinsso</span></td>
          <td><span class="warrior">Warrior</span></td>
          <td>250</td>
        </tr>
        <tr>
          <td>10</td>
          <td><a href="">Vex</a></td>
          <td><span class="clan">Shinsso</span></td>
          <td><span class="warrior">Warrior</span></td>
          <td>250</td>
        </tr>
      </tbody>
    </table>
  </div>
  <div class="topHome-50">
    <div class="topHome-title flex-s-c">
      <span>TOP Guilds</span> <a href="" class="button button-small">View More</a>
    </div>
    <table class="top-table">
      <thead>
        <tr>
          <td>#</td>
          <td>Name</td>
          <td>Empire</td>
          <td>Race</td>
          <td>Level</td>
        </tr>
      </thead>
      <tbody>
        <tr>
          <td>1</td>
          <td><a href="">Designers</a></td>
          <td><span class="clan">Shinsso</span></td>
          <td><a href="">Vex</a></td>
          <td>250</td>
        </tr>
        <tr>
          <td>2</td>
          <td><a href="">Designers</a></td>
          <td><span class="clan">Shinsso</span></td>
          <td><a href="">Vex</a></td>
          <td>250</td>
        </tr>
        <tr>
          <td>3</td>
          <td><a href="">Designers</a></td>
          <td><span class="clan">Shinsso</span></td>
          <td><a href="">Vex</a></td>
          <td>250</td>
        </tr>
        <tr>
          <td>4</td>
          <td><a href="">Designers</a></td>
          <td><span class="clan">Shinsso</span></td>
          <td><a href="">Vex</a></td>
          <td>250</td>
        </tr>
        <tr>
          <td>5</td>
          <td><a href="">Designers</a></td>
          <td><span class="clan">Shinsso</span></td>
          <td><a href="">Vex</a></td>
          <td>250</td>
        </tr>
        <tr>
          <td>6</td>
          <td><a href="">Designers</a></td>
          <td><span class="clan">Shinsso</span></td>
          <td><a href="">Vex</a></td>
          <td>250</td>
        </tr>
        <tr>
          <td>7</td>
          <td><a href="">Designers</a></td>
          <td><span class="clan">Shinsso</span></td>
          <td><a href="">Vex</a></td>
          <td>250</td>
        </tr>
        <tr>
          <td>8</td>
          <td><a href="">Designers</a></td>
          <td><span class="clan">Shinsso</span></td>
          <td><a href="">Vex</a></td>
          <td>250</td>
        </tr>
        <tr>
          <td>9</td>
          <td><a href="">Designers</a></td>
          <td><span class="clan">Shinsso</span></td>
          <td><a href="">Vex</a></td>
          <td>250</td>
        </tr>
        <tr>
          <td>10</td>
          <td><a href="">Designers</a></td>
          <td><span class="clan">Shinsso</span></td>
          <td><a href="">Vex</a></td>
          <td>250</td>
        </tr>
      </tbody>
    </table>
  </div>
</div>

<div class="top-all-button">
  <a href="" class="button">View All Rankings</a>
</div>


</div>
</template>
<script>
  // import HomeLanding from "@/views/homePage/HomeLanding.vue";


  export default {
    name: "index",
    components: {},
    data() {
      return {
        banners : [
          {img: 'slider-img.jpg'},
          {img: 'slider-img-3.jpg'},
          {img: 'slider-img-2.jpg'},

        ],
        options : {
              rewind : true,
              perPage: 1,
              // gap    : '1rem',
              autoplay: true,
              pagination: true,
              breakpoints: {
                  1080: {
                      perPage: 2
                  },
                  756: {
                      perPage: 1
                  }
              },
          },
      }
    }
  };
</script>
<style lang="css">
  /* .splide-list {
    backface-visibility: hidden;
    display: flex;
    height: 100%;
    margin: 0!important;
    padding: 0!important;
    transform-style: preserve-3d;
  }
  .splide__arrow{
    border-radius: 25%;
    background: #93acd3;
    
  }
  .splide__slide {
    margin-right: 16px;
  } */
</style>