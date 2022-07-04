<template>
  <div>
    <JumboSection></JumboSection>
    <EnrollSection></EnrollSection>
    <WelcomeSection></WelcomeSection>
    <CarouselSection></CarouselSection>
  </div>
</template>

<script>
import JumboSection from "./JumboSection.vue";
import EnrollSection from "./EnrollSection.vue";
import WelcomeSection from "./WelcomeSection.vue";
import CarouselSection from "./CarouselSection.vue";
export default {
  name: "TheMain",
  components: { JumboSection, EnrollSection, WelcomeSection, CarouselSection },
};
</script>

<style scoped lang="scss"></style>
