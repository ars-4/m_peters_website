<template>
  <div class="home">
    <div class="row intro-section">
      <div class="col-md-6 image">
        <div class="box">
          <div class="boxOne">
            <div class="boxTwo"></div>
          </div>
        </div>
      </div>
      <div class="col-md-6 content">
        <br>
        <div class="box">
          <div class="boxOne">
            <h1>The About</h1>
            <p>
              Lorem ipsum dolor sit amet consectetur adipisicing elit. Rerum nihil praesentium, perspiciatis voluptates
              quae
              deleniti modi eum quod reiciendis expedita voluptate asperiores a esse natus ducimus fuga? Vitae, nemo
              libero.
              Lorem ipsum dolor sit amet consectetur adipisicing elit. Nobis vel impedit fugiat iusto laborum enim
              deleniti, excepturi non aperiam! Tempora pariatur quo incidunt beatae reprehenderit, fugit error cupiditate
              asperiores sed.
            </p>
            <div class="buttons">
              <button class="btn btn-primary">Learn More</button>
              <button class="btn btn-primary">Read More</button>
            </div>
          </div>
        </div>
      </div>
    </div>

    <div class="gallery-section">
      <div class="headers">
        <h1>Gallery</h1>
        <router-link to="/gallery">View All -></router-link>
      </div>
      <div class="galleryImages">
        <div class="row">
          <div class="col-md-3">
            <div class="imageBox">
              <div class="boxOne">
                <div class="boxTwo"></div>
              </div>
            </div>
          </div>
          <div class="col-md-3">
            <div class="imageBox">
              <div class="boxOne">
                <div class="boxTwo"></div>
              </div>
            </div>
          </div>
          <div class="col-md-3">
            <div class="imageBox">
              <div class="boxOne">
                <div class="boxTwo"></div>
              </div>
            </div>
          </div>
          <div class="col-md-3">
            <div class="imageBox">
              <div class="boxOne">
                <div class="boxTwo"></div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>

    <div class="continued-section">
      <div class="dumb_box"></div>
      <div class="box">
        <div class="boxOne">
          <div class="boxTwo">
            <div class="boxThree">
              <h1>Learn More?</h1>
              <p>
                Lorem ipsum, dolor sit amet consectetur adipisicing elit. Numquam iure soluta, velit excepturi corporis
                sint
                voluptas nulla optio ipsum vitae tenetur quod perspiciatis. Voluptates voluptate totam ea ullam quasi
                soluta.
                Lorem ipsum dolor sit amet consectetur, adipisicing elit. Totam at inventore quaerat ducimus sed sunt
                soluta
                saepe
                praesentium dolore, sint adipisci, ex, eveniet architecto ipsam commodi voluptatem incidunt corrupti
                cupiditate!
              </p>
              <div class="form">
                <input type="text" class="form-control" placeholder="Enter Your Email">
                <button class="btn btn-primary">Register</button>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style>
.home {
  padding: 0px 10px;
  overflow-x: hidden !important;
}

.home .intro-section {
  position: relative;
  background-color: var(--bg-primary);
  color: var(--text-secondary);
}

.home .intro-section::after{
  background-color: var(--bg-primary);
  content: '';
  width: 200%;
  height: 100%;
  top: 25%;
  left: -10%;
  z-index: -1;
  transform: rotate(10deg);
  position: absolute;
}

.home .intro-section .image .box,
.home .intro-section .content .box,
.gallery-section .galleryImages .col-md-3 .imageBox,
.continued-section .box {
  position: relative;
  width: 100%;
  display: flex;
  justify-content: center;
  align-items: center;
  aspect-ratio: 4/3;
}

.home .intro-section .image .box .boxOne,
.gallery-section .galleryImages .col-md-3 .imageBox .boxOne,
.continued-section .box .boxOne {
  position: relative;
  width: 50%;
  aspect-ratio: 4/4;
  border: 1px solid #242424;
  border-radius: 4px;
  background-color: #c4b9c4;
}

.home .intro-section .image .box .boxTwo,
.gallery-section .galleryImages .col-md-3 .imageBox .boxOne .boxTwo,
.continued-section .box .boxTwo {
  position: absolute;
  top: 5%;
  left: 5%;
  background-color: #242424;
  width: 100%;
  aspect-ratio: 4/4;
  border: 1px solid #242424;
  border-radius: 4px;
}

.home .intro-section .content .box .boxOne {
  text-align: center;
  width: 75%;
  aspect-ratio: 5/3;
  border-radius: 4px;
}

.home .intro-section .content .box .boxOne .btn {
  margin: 0px 8px;
}


/* Gallery */
.gallery-section {
  width: 100%;
  /* height: 200px;
  overflow-y: hidden !important; */
}
.gallery-section .headers {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 0px 20px;
}

.gallery-section .headers h1 {
  mix-blend-mode: difference;
  color: #fff;
}

.gallery-section .galleryImages .col-md-3 .imageBox {
  aspect-ratio: 4/1 !important;
  margin-bottom: 18px;
}

.gallery-section .galleryImages .col-md-3 .imageBox .boxOne {
  width: 90%;
  border: 1px solid #242424;
}


.continued-section {
  /* display: none; */
  /* overflow-y: hidden !important; */
  padding: 60px 0px;
  position: relative;
  background-color: #242424;
  margin-left: -1%;
  width: 103%;
  margin-bottom: 0;
  margin-top: 5%;
}
.continued-section .dumb_box {
  position: absolute;
  top: -10%;
  left: -10%;
  transform: rotate(10deg);
  background-color: #242424;
  width: 40%;
  height: 40%;
}

.continued-section .box {
  aspect-ratio: 4/1;
}

.continued-section .box .boxOne {
  width: 75%;
  aspect-ratio: 4/1;
}

.continued-section .box .boxTwo {
  width: 100%;
  aspect-ratio: 4/1;
  text-align: center;
  display: flex;
  justify-content: center;
  align-items: center;
}

.continued-section .box .boxTwo .boxThree {
  display: block;
  color: var(--text-secondary);
  padding: 10px 30px;
}

.continued-section .box .boxTwo .boxThree .form {
  display: flex;
  margin: 0px 25%;
  justify-content: space-between;
  align-items: center;
}

.continued-section .box .boxTwo .boxThree .form input {
  margin-right: 8px;
}


@media screen and (max-width:700px) {
  .home .intro-section .image .box .boxOne {
    width: 75%;
  }

  .home .intro-section .content .box .boxOne,
  .home .continued-section .box .boxOne {
    width: 90%;
  }

  .home .intro-section .content .box .boxOne .btn {
    width: 100%;
    margin: 8px 0px;
  }

  .continued-section {
    margin-left: -4%;
    width: 108%;
  }
  .continued-section .dumb_box {
    top: -3% !important;
    left: -8% !important;
    width: 80% !important;
  }

  .continued-section .box {
    width: 106%;
    margin-left: -3%;
    font-size: 12px;
    aspect-ratio: 4/5;
  }

  .home .continued-section .box .boxOne {
    margin-left: -4%;
    aspect-ratio: 4/5;
  }

  .home .continued-section .box .boxOne .form {
    display: block;
    margin-left: 3%;
    margin-right: 3%;
  }

  .home .continued-section .box .boxOne .form .btn {
    margin-top: 8px;
    width: 100%;
  }

}
</style>

<script>
import { defineComponent } from 'vue';
import AdBox from '@/components/AdComponent.vue'

export default defineComponent({
  components: {
    AdBox
  }
})

</script>