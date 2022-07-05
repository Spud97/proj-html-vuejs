<template>
  <div class="pt-3">
    <div class="container padd d-flex flex-column align-items-center">
      <h2 class="title">Welcome to Fable</h2>
      <span class="text-grey pb-4"
        >Fable daycare, preschool, and kindergarten</span
      >
      <img
        id="divider"
        src="../../public/images/header_divider.png"
        alt="divider"
        class="mb-4"
      />
      <div class="container-fluid my-pt">
        <div class="row row-cols-4">
          <div class="col">
            <div class="my-card d-flex flex-column align-items-center">
              <div
                class="box-img bg-orange d-flex justify-content-center align-items-center mb-3"
              >
                <img
                  src="../../public/images/schoolbag_alt.png"
                  alt=""
                  class="card-img"
                />
              </div>
              <h5 class="title text-center pb-2">Morbi Etos</h5>
              <p class="text-center text-secondary small-font">
                Praesent interdum est gravida vehicula est node maecenas loareet
                morbi a dosis luctus novum est praesent.
              </p>
            </div>
          </div>
          <div class="col">
            <div class="my-card d-flex flex-column align-items-center">
              <div
                class="box-img bg-blue d-flex justify-content-center align-items-center mb-3"
              >
                <img
                  src="../../public/images/stroller_alt.png"
                  alt=""
                  class="card-img"
                />
              </div>
              <h5 class="title text-center pb-2">Congue Gravida</h5>
              <p class="text-center text-secondary small-font">
                Elipsis magna a terminal nulla elementum morbi elite forte
                maecenas est magna etos interdum vitae est.
              </p>
            </div>
          </div>
          <div class="col">
            <div class="my-card d-flex flex-column align-items-center">
              <div
                class="box-img bg-orange d-flex justify-content-center align-items-center mb-3"
              >
                <img
                  src="../../public/images/globe_alt.png"
                  alt=""
                  class="card-img"
                />
              </div>
              <h5 class="title text-center pb-2">Maecenas Node</h5>
              <p class="text-center text-secondary small-font">
                Praesent interdum est gravida vehicula est node maecenas loareet
                morbi a dosis luctus novum est praesent.
              </p>
            </div>
          </div>
          <div class="col">
            <div class="my-card d-flex flex-column align-items-center">
              <div
                class="box-img bg-blue d-flex justify-content-center align-items-center mb-3"
              >
                <img
                  src="../../public/images/bell_alt.png"
                  alt=""
                  class="card-img"
                />
              </div>
              <h5 class="title text-center pb-2">Praesent Morbi</h5>
              <p class="text-center text-secondary small-font">
                Elipsis magna a terminal nulla elementum morbi elite forte
                maecenas est magna etos interdum vitae est.
              </p>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "WelcomeSection",
};
</script>

<style scoped lang="scss">
h2 {
  font-family: "Raleway", sans-serif;
  font-size: 2.5rem;
}
#divider {
  height: 0.7rem;
}
.padd {
  padding: 30px 250px;
}
.my-pt {
  padding-top: 30px;
}
.title {
  color: #56509f;
}
.text-grey {
  color: rgb(168, 168, 168);
}
.small-font {
  font-size: 0.8rem;
}
.box-img {
  border: 1px solid transparent;
  border-radius: 50%;
  height: 140px;
  width: 140px;
}
.card-img {
  height: 50px;
  width: 50px;
}
.bg-orange {
  background-color: #fe6500;
}
.bg-blue {
  background-color: #56509f;
}
</style>
