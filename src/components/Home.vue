
<template>
  <div class="header">
    <div class="menu">
      <div class="logo">
        <img alt="Vue logo" src="../assets/Cotral_logo.png" />
      </div>
      <ul>
        <li><a href="#">Home</a></li>
        <li><a href="#">About us</a></li>
        <li><a href="#">Contact us</a></li>
      </ul>
    </div>
    <div class="headerContent">
      <h1>Magna Aliquam</h1>
      <p>Sed lorem ipsum sed dolor nullam adipiscing</p>
      <button>LEARN MORE</button>
    </div>
  </div>
  <div class="sliderContent">
    <h2>Lorem ipsum dolor</h2>
    <p>
      Ipsum dolor tempus commodo turpis adipiscing adipiscing in tempor placerat
      sed amet accumsan enim lorem sem turpis ut. Massa amet erat accumsan curae
      blandit porttitor faucibus in nisl nisi volutpat massa mi non nascetur.
    </p>
    <div class="sliderMain">
      <div class="slider">
        <img src="../assets/unnamed.jpg" alt="" />
        <img src="../assets/download.jpeg" alt="" />
        <img src="../assets/1866762.jpg" alt="" />
      </div>
      <div class="sliderArrow">
        <font-awesome-icon v-on:click="left" class="left" icon="chevron-left" />
        <font-awesome-icon
          v-on:click="right"
          class="right"
          icon="chevron-right"
        />
      </div>
    </div>
  </div>
  <div class="posts">
    <h1>All Posts</h1>
    <div class="allPost">
      <div class="post">
        <img src="../assets/post-instagram-1.jpg" alt="" />
        <h3>Sed amet lorem</h3>
        <p>
          Ipsum dolor tempus et commodo lorem accumsan et adipiscing blandit
          porttitor.
        </p>
        <button>LEARN MORE</button>
      </div>
      <div class="post">
        <img src="../assets/post-instagram-1.jpg" alt="" />
        <h3>Sed amet lorem</h3>
        <p>
          Ipsum dolor tempus et commodo lorem accumsan et adipiscing blandit
          porttitor.
        </p>
        <button>LEARN MORE</button>
      </div>
      <div class="post">
        <img src="../assets/post-instagram-1.jpg" alt="" />
        <h3>Sed amet lorem</h3>
        <p>
          Ipsum dolor tempus et commodo lorem accumsan et adipiscing blandit
          porttitor.
        </p>
        <button>LEARN MORE</button>
      </div>
      <div class="post">
        <img src="../assets/post-instagram-1.jpg" alt="" />
        <h3>Sed amet lorem</h3>
        <p>
          Ipsum dolor tempus et commodo lorem accumsan et adipiscing blandit
          porttitor.
        </p>
        <button>LEARN MORE</button>
      </div>
      <div class="post">
        <img src="../assets/post-instagram-1.jpg" alt="" />
        <h3>Sed amet lorem</h3>
        <p>
          Ipsum dolor tempus et commodo lorem accumsan et adipiscing blandit
          porttitor.
        </p>
        <button>LEARN MORE</button>
      </div>
    </div>
    
  </div>
</template>
<script>
import "./Style.css";
export default {
  methods: {
    left() {
      const imgWidth = document.querySelector(".slider img").width;
      document.querySelector(".slider").scrollLeft -= imgWidth;
    },
    right() {
      const imgWidth = document.querySelector(".slider img").width;
      document.querySelector(".slider").scrollLeft += imgWidth;
    },
  },
};
</script>
