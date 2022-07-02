<template>
  <div>
    <div class="debug container padd d-flex justify-content-between">
      <div>
        <img src="../../public/images/logo.png" alt="logo-header" />
      </div>
      <div class="d-flex align-items-center text-blue">
        <div
          v-for="link in linkList"
          :key="link.id"
          class="text-center d-flex flex-column justify-content-center"
          :class="{ activeLink: link.active == true }"
        >
          <i :class="link.icon" class="pb-2 p-link"></i>
          <span class="pt-1">{{ link.name }}</span>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "TheHeader",
  data() {
    return {
      linkList: [
        {
          name: "Home",
          icon: "fa-solid fa-house",
          id: 0,
          active: true,
        },
        {
          name: "Pages",
          icon: "fa-solid fa-file-lines",
          id: 1,
          active: false,
        },
        {
          name: "Blog",
          icon: "fa-solid fa-file-invoice",
          id: 2,
          active: false,
        },
        {
          name: "Shop",
          icon: "fa-solid fa-cart-shopping",
          id: 3,
          active: false,
        },
        {
          name: "Shortcodes",
          icon: "fa-solid fa-flask",
          id: 4,
          active: false,
        },
        {
          name: "Support",
          icon: "fa-solid fa-message",
          id: 5,
          active: false,
        },
        {
          name: "Contact",
          icon: "fa-solid fa-envelope",
          id: 6,
          active: false,
        },
      ],
    };
  },
};
</script>

<style scoped lang="scss">
img {
  height: 6rem;
}
i {
  font-size: 1.5rem;
}
span {
  font-size: 0.8rem;
}
.debug {
  border: 1px dashed red;
}
.padd {
  padding: 0px 250px;
}
.text-blue {
  color: #56509f;
}
.p-link {
  padding: 0px 29px;
}
.activeLink {
  color: white;
  background-color: #fd6500;
  height: 100%;
}
</style>
