<template>
  <div class="bg-section py-4">
    <div class="container padd">
      <div class="row row-cols-2 py-3">
        <div class="col">
          <div class="d-flex flex-column pe-2">
            <div class="d-flex flex-row position-relative pb-1">
              <div id="overview" class="bg-orange text-white py-2 px-4">
                Overview
              </div>
              <div id="triangle" class="bg-orange"></div>
              <div id="our-mission" class="text-grey py-2 px-3">
                Our Mission
              </div>
            </div>
            <p class="title medium-font pt-4">
              Our philosophy is learning through play as we offer a stimulating
              environment for children.
            </p>
            <div class="d-flex">
              <div
                class="box-icon bg-orange d-flex align-items-center justify-content-center"
              >
                <img
                  class="icon"
                  src="../../public/images/clock_alt.png"
                  alt="icon"
                />
              </div>
              <div class="ps-4 d-flex flex-column">
                <h5 class="title">Full Day Sessions</h5>
                <p class="small-font text-dark-grey pt-1 my-text">
                  Pulvinar est metro ligula blandit maecenas retrum gravida
                  cuprum. Maecenas node estibulum.
                </p>
              </div>
            </div>
            <div class="d-flex">
              <div
                class="box-icon bg-orange d-flex align-items-center justify-content-center"
              >
                <img
                  class="icon"
                  src="../../public/images/diagram_alt.png"
                  alt="icon"
                />
              </div>
              <div class="ps-4 d-flex flex-column">
                <h5 class="title">Varied Classes</h5>
                <p class="small-font text-dark-grey pt-1 my-text">
                  Pulvinar est metro ligula blandit maecenas retrum gravida
                  cuprum. Maecenas node estibulum.
                </p>
              </div>
            </div>
          </div>
        </div>
        <div class="col">
          <div class="d-flex flex-column">
            <div id="main-img">
              <div
                class="slide-btn prev bg-orange d-flex align-items-center justify-content-center"
              >
                <img src="../../public/images/slider_previous.png" alt="" />
              </div>
              <div
                class="slide-btn next bg-orange d-flex align-items-center"
              >
                <img src="../../public/images/slider_next.png" alt="" />
              </div>
            </div>

            <div
              class="row row-cols-3 pt-2 px-2 justify-content-center"
            >
              <div class="col d-flex justify-content-center px-0">
                <div id="slide-1" class="slide"></div>
              </div>
              <div class="col d-flex justify-content-center px-0 outline">
                <div id="slide-2" class="slide"></div>
              </div>
              <div class="col d-flex justify-content-center px-0">
                <div id="slide-3" class="slide"></div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "CarouselSection",
};
</script>

<style scoped lang="scss">
#triangle {
  transform: rotate(45deg);
  height: 30px;
  width: 30px;
  position: absolute;
  top: 10px;
  left: 42px;
  z-index: 0;
}
#overview {
  z-index: 1;
}
#our-mission {
  border-bottom: 2px solid rgb(237, 237, 237);
  margin-left: 25px;
}
#main-img {
  background-image: url("../../public/images/gallery_01-690x506.jpg");
  height: 270px;
  background-size: cover;
  position: relative;
}
#slide-1 {
  background-image: url("../../public/images/gallery_07-690x506.jpg");
}
#slide-2 {
  background-image: url("../../public/images/gallery_01-690x506.jpg");
}
#slide-3 {
  background-image: url("../../public/images/gallery_08-690x506.jpg");
}
.padd {
  padding: 30px 250px;
}
.title {
  color: #56509f;
}
.text-grey {
  color: rgb(168, 168, 168);
}
.text-dark-grey {
  color: rgb(139, 139, 139);
}
.small-font {
  font-size: 0.8rem;
}
.medium-font {
  font-size: 1.4rem;
}
.bg-orange {
  background-color: #fe6500;
}
.bg-section {
  background-color: #f5f5f5;
}
.box-icon {
  height: 60px;
  width: 60px;
  border: 1px solid transparent;
  border-radius: 50%;
}
.icon {
  height: 25px;
}
.my-text {
  width: 300px;
}
.slide {
  height: 90px;
  width: 94%;
  background-size: cover;
}
.slide-btn {
  height: 40px;
  width: 40px;
  position: absolute;
  top: 50%;
  transform: translate(0%, -50%);
  cursor: pointer;
}
.prev {
  left: 0px;
}
.next {
  right: 0px;
}
.outline {
  padding-bottom: 7px;
  border-bottom: 2px solid #fe6500;
}
</style>
