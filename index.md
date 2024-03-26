---
layout: default
title: Home
underConstruction: assets/images/work.jpg
imageOpacity: 0.8
---

<style>
/* Carousel */
.carousel-control-prev-icon {
    width: 60px;
    height: 60px;
}
    
.carousel-control-next-icon {
    width: 60px;
    height: 60px;
}

.carousalContainer {
    min-width: 90vw;
    max-height: 50vh;
    text-align: center;
    /* tweaks */
    margin-top: 100px; /* for iphone SE resolution */
}
@media (max-width: 767px) {
    .carousalContainer {
        min-width: 90vw;
        max-height: 50vh;
        text-align: center;
        /* tweaks */
        margin-top: 100px; /* for iphone SE resolution */
    }
}

.carousel-item img {
    /* object-fit: fill; */
    min-width: 90vw;
    max-height: 50vh;
    text-align: center;
}

.center-content {
    height: calc(100vh - 60vh);
    display: flex;
    justify-content: center;
    align-items: center;
    /* text styling */
    font-size: 3em;
    text-align: center;
    overflow: hidden;
}

@media (max-width: 767px) {
    .center-content {
        height: calc(100vh - 75vh);
        display: flex;
        justify-content: center;
        align-items: center;
        /* text styling */
        font-size: 2em;
        text-align: center;
        overflow: hidden;
        /* tweaks */
        margin-top: 10px;
    }
}

/* OTHER TRIES */
.message {
    min-width: 100vw;
    max-height: calc(100vh - 60vh);
}

.center-parent {
    background: gray;
    height: 100%;
    width: 100%;
    position: relative;
}
.center-child {
    background-color: orange;
    width: 100%;
    height: 100%;
    position: absolute;
    top: 50%;
    left: 50%;
    /* margin: 0px auto; */
    transform: translate(-50%, -50%);
    -webkit-transform: translate(-50%, -50%);
    /* max-width: 100%;
    max-height: 100%;
    overflow: hidden; */
}
</style>

<div class="carousalContainer">
    <div id="carouselExampleCaptions" class="carousel carousel-dark slide" data-bs-ride="carousel" data-bs-touch="true" data-bs-interval="true">
        <div class="carousel-indicators">
          <button type="button" data-bs-target="#carouselExampleCaptions" data-bs-slide-to="0" class="active" aria-current="true" aria-label="Slide 1"></button>
          <button type="button" data-bs-target="#carouselExampleCaptions" data-bs-slide-to="1" aria-label="Slide 2"></button>
          <button type="button" data-bs-target="#carouselExampleCaptions" data-bs-slide-to="2" aria-label="Slide 3"></button>
        </div>
        <div class="carousel-inner">
          <div class="carousel-item active" data-bs-interval="3000">
            <img src="{{page.underConstruction}}" class="img-fluid" alt="..." style="opacity:{{page.imageOpacity}}">
            <div class="carousel-caption d-none d-md-block">
              <h1>Under Construction</h1>
              <p>Work in progress</p>
            </div>
          </div>
          <div class="carousel-item" data-bs-interval="3000">
            <img src="{{page.underConstruction}}" class="img-fluid" alt="..." style="opacity:{{page.imageOpacity}}">
            <div class="carousel-caption d-none d-md-block">
              <h1>Under Construction</h1>
              <p>Work in progress</p>
            </div>
          </div>
          <div class="carousel-item" data-bs-interval="3000">
            <img src="{{page.underConstruction}}" class="img-fluid" alt="..." style="opacity:{{page.imageOpacity}}">
            <div class="carousel-caption d-none d-md-block">
              <h1>Under Construction</h1>
              <p>Work in progress</p>
            </div>
          </div>
        </div>
        <button class="carousel-control-prev" type="button" data-bs-target="#carouselExampleCaptions" data-bs-slide="prev">
          <span class="carousel-control-prev-icon" aria-hidden="true"></span>
          <span class="visually-hidden">Previous</span>
        </button>
        <button class="carousel-control-next" type="button" data-bs-target="#carouselExampleCaptions" data-bs-slide="next">
          <span class="carousel-control-next-icon" aria-hidden="true"></span>
          <span class="visually-hidden">Next</span>
        </button>
      </div>
</div>

{% comment %} <div class="message">
    <div class="center-parent">
        <div class="center-child">
            <div style="font-size: 3em;">
                Under Construction
            </div>
        </div>
    </div>
</div> {% endcomment %}

<div class="center-content">
    The site is under development and will be up soon... :)
</div>