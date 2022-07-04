<template>
  <div>
    <div class="container padd d-flex justify-content-between">
      <div>
        <img id="logo" src="../../public/images/logo.png" alt="logo-header" />
      </div>
      <div class="d-flex align-items-center text-blue">
        <div
          v-for="link in linkList"
          :key="link.id"
          class="text-center d-flex flex-column justify-content-center align-items-center pointer px-1"
          :class="{ activeLink: link.active == true }"
        >
          <img :src="`../../images${link.icon}`" alt="icon" class="icon-header my-2 mx-4">
          <span class="icon-padding">{{ link.name }}</span>
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
          icon: "/home-2.png",
          id: 0,
          active: true,
        },
        {
          name: "Pages",
          icon: "/document.png",
          id: 1,
          active: false,
        },
        {
          name: "Blog",
          icon: "/printer.png",
          id: 2,
          active: false,
        },
        {
          name: "Shop",
          icon: "/cart.png",
          id: 3,
          active: false,
        },
        {
          name: "Shortcodes",
          icon: "/lab.png",
          id: 4,
          active: false,
        },
        {
          name: "Support",
          icon: "/chat.png",
          id: 5,
          active: false,
        },
        {
          name: "Contact",
          icon: "/envelope.png",
          id: 6,
          active: false,
        },
      ],
    };
  },
};
</script>

<style scoped lang="scss">
i {
  font-size: 1.5rem;
}
span {
  font-size: 0.8rem;
}
#logo {
  height: 6rem;
}
.padd {
  padding: 0px 250px;
}
.text-blue {
  color: #56509f;
}
.activeLink {
  color: white;
  background-color: #fd6500;
  height: 100%;
}
.icon-header {
  height: 1.5rem;
  width: 1.5rem;
}
.icon-padding {
  padding: 5px 0px 10px 0px;
}
.pointer {
  cursor: pointer;
}
</style>
