<template>
  <div>
    <JumboSection></JumboSection>
    <EnrollSection></EnrollSection>
    <WelcomeSection></WelcomeSection>
  </div>
</template>

<script>
import JumboSection from "./JumboSection.vue";
import EnrollSection from "./EnrollSection.vue";
import WelcomeSection from "./WelcomeSection.vue";
export default {
  name: "TheMain",
  components: { JumboSection, EnrollSection, WelcomeSection },
};
</script>

<style scoped lang="scss"></style>
