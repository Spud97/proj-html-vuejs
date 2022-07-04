<template>
  <div class="bg-jumbo">
    <div class="container h-100 position-relative d-flex align-items-end justify-content-center">
      <img id="train" src="../../public/images/slider_slide3_img2.png" alt="">
      <img id="blocks" src="../../public/images/slider_slide3_img3.png" alt="">
      <span id="text-jumbo">Learning & Fun</span>
      <div class="jumbo-slides"></div>
      <div class="jumbo-slides mx-2"></div>
      <div id="active-slide" class="jumbo-slides"></div>
    </div>
  </div>
</template>

<script>
export default {
  name: "JumboSection",
};
</script>

<style scoped lang="scss">
#train {
  height: 130px;
  position: absolute;
  bottom: 50px;
  left: 500px;
}
#blocks {
  height: 90px;
  position: absolute;
  bottom: 45px;
  right: 140px;
}
#text-jumbo {
  font-family: 'Handlee', cursive;
  font-size: 1.9rem;
  color: #eae4e0;
  position: absolute;
  top: 120px;
  left: 250px;
}
#active-slide {
  margin-bottom: 35px;
}
.padd {
  padding: 0px 250px;
}
.bg-jumbo {
  background-image: url("../../public/images/slider_slide3_background.png");
  height: 480px;
  background-position-y: -80px;
}
.jumbo-slides {
  border: 2px solid #fd6500;
  height: 10px;
  width: 33px;
  margin-bottom: 26px;
}
</style>
