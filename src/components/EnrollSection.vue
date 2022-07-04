<template>
  <div class="bg-section">
    <div class="container padd d-flex justify-content-between">
      <h3 class="text-white m-0">How to Enroll Your Child to a Class?</h3>
      <button class="button">
        LEARN MORE <i class="fa-solid fa-angle-right ps-2"></i>
      </button>
    </div>
  </div>
</template>

<script>
export default {
  name: "EnrollSection",
};
</script>

<style scoped lang="scss">
h3 {
  font-family: "Raleway", sans-serif;
}
.padd {
  padding: 30px 250px;
}
.bg-section {
  background-image: url("../../public/images/pattern.png");
}
.button {
  padding: 0.6rem 1rem;
  text-align: center;
  border: 2px solid white;
  background-color: transparent;
  font-weight: bold;
  font-size: 0.7rem;
  color: white;
}
.button:hover {
  background-color: white;
  color: #56509f;
}
</style>
