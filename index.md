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
/* Cards - Branch Hyperlinks */
.card-container {
    display: flex;
    flex-wrap: wrap;
    justify-content: center; /* Center horizontally */
    min-width: 80vw;
    margin: 10%;
}

.card {
    width: calc(25% - 20px); /* Make the cards smaller and adjust margin */
    margin: 10px;
    height: 300px; /* Set a fixed height for the cards */
    display: flex;
    flex-direction: column;
    overflow: hidden; /* Hide overflow content */
    justify-content: center; /* Center content vertically */
    align-items: center; /* Center content horizontally */
    text-align: center; /* Center text horizontally */
    transition: transform 0.3s ease; /* Add transition for smooth animation */
}

.card:hover {
    transform: scale(1.05); /* Scale up the card slightly on hover */
}

.card a {
    text-decoration: none; /* Remove default underline */
    color: inherit; /* Inherit text color from parent */
}

.card img {
    width: 100%; /* Ensure image takes up full width of card */
    height: 50%; /* Ensure image takes up full height of card */
    object-fit: fill; /* Maintain aspect ratio while covering the entire space */
}

.card h2, .card p {
    margin-top: 20px; /* Remove default margin for title and description */
}

@media screen and (max-width: 768px) {
    .card {
        width: calc(30% - 20px); /* Adjust width for 3 cards per row on smaller screens */
    }
}

@media screen and (max-width: 480px) {
    .card {
        width: calc(80% - 20px); /* Adjust width for 1 card per row on mobile */
    }
}

/* Cards - Address */
.address-block-container {
    display: flex;
    flex-wrap: wrap;
    justify-content: flex-start; /* space-evenly; space-between; Distribute blocks evenly */
    min-width: 80vw;
    margin: 3%;
}

.address-block {
    width: calc(25% - 20px); /* Initial width for desktop (4 blocks in a row) */
    margin: 10px;
    padding: 20px;
    border: 1px solid #ccc;
    border-radius: 5px;
    background-color: #f9f9f9;
    color: black;
    box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
    transition: width 0.3s ease; /* Transition for resizing */
}

@media screen and (max-width: 1200px) {
    .address-block {
        width: calc(33.33% - 20px); /* Adjust width for 3 blocks in a row on smaller screens */
    }
}

@media screen and (max-width: 992px) {
    .address-block {
        width: calc(50% - 20px); /* Adjust width for 2 blocks in a row on smaller screens */
    }
}

@media screen and (max-width: 768px) {
    .address-block {
        width: calc(100% - 20px); /* Full width for 1 block per row on mobile */
    }
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

<div class="card-container">
    {% for card in site.data.cards %}
    <div class="card">
      <a href="#">
        <img src="{{ card.image }}" alt="{{ card.title }}">
        <h2>{{ card.title }}</h2>
        <p>{{ card.description }}</p>
      </a>
    </div>
    {% endfor %}
</div>

<div style="background-color: lightgray;">
  <h1 style="text-align: center;">Branch Details</h1>

  <div class="address-block-container">
      {% for addressBlock in site.data.addressBlocks.list %}
        <div class="address-block">
            <div class="address-details">
                <h6><strong>{{ addressBlock.title }}</strong></h6>
                <p style="margin: 0"><strong>{{ addressBlock.location.title }}:</strong> {{ addressBlock.location.value }}</p>
                <p style="margin: 0"><strong>{{ addressBlock.mobile.title }}:</strong> {{ addressBlock.mobile.value }}</p>
                <p style="margin: 0"><strong>{{ addressBlock.email.title }}:</strong> {{ addressBlock.email.value }}</p>
            </div>
        </div>
      {% endfor %}
  </div>
  <div class="mb-5">&nbsp;</div>
</div>


<!-- <div class="center-content">
    The site is under development and will be up soon... :)
</div> -->

<!-- <div class="message">
    <div class="center-parent">
        <div class="center-child">
            <div style="font-size: 3em;">
                Under Construction
            </div>
        </div>
    </div>
</div> -->

