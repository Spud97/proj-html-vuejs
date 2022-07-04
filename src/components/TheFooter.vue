<template>
  <div>
    <div class="bg-footer">
      <div class="debug container padd pb-5">
        <div class="row row-cols-4 pb-5">
          <div class="col px-0">
            <div class="debug text-white pt-4 px-3">
              <h4 class="pt-3">ABOUT US</h4>
              <hr />
              <p class="footer-text-color small-font pt-2">
                Elipsis magna a nulla elite forte maecenas est elementum magna
                etos interdum movum morbi vehicula morbi.
              </p>
              <img
                id="logo-footer"
                src="../../public/images/logo_footer.png"
                alt="logo-footer"
              />
            </div>
          </div>
          <div class="col px-0">
            <div class="debug text-white pt-4 ps-3 pe-1">
              <h4 class="pt-3">ARCHIVES</h4>
              <hr />
              <div class="pt-2">
                <div
                  v-for="archive in archivesList"
                  :key="archive.id"
                  class="text-center d-flex footer-text-color archive-box mb-1"
                >
                  <span class="small-font bold"
                    >{{ archive.date.toUpperCase() }} ({{
                      archive.number
                    }})</span
                  >
                </div>
              </div>
            </div>
          </div>
          <div class="col px-0">
            <div class="debug text-white pt-4 px-3">
              <h4 class="pt-3">OUR FEATURES</h4>
              <hr />
              <p class="footer-text-color small-font pt-2">
                Nunc grovida rutrum maurs vehin hasellus ac pretium aupue
                vhvamul lacus ligul mattis ac vene:
              </p>
              <ul>
                <li
                  v-for="feature in featuresList"
                  :key="feature.text"
                  class="footer-text-color small-font py-1"
                >
                  <img
                    src="../../public/images/style_4_alt.png"
                    alt="check"
                    class="check-box pe-1"
                  />
                  {{ feature.text }}
                </li>
              </ul>
            </div>
          </div>
          <div class="col px-0">
            <div class="debug text-white pt-4 px-3">
              <h4 class="pt-3">RECENT POSTS</h4>
              <hr />
              <div>
                <div v-for="post in postsList" :key="post.title" class="d-flex">
                  <img :src="`../../public/images${post.img}`" alt="post-thumbnails" />
                  <div class="d-flex flex-column">
                    <span class="medium-font">{{ post.title }}</span>
                    <div class="d-flex">
                      <img
                        src="../../public/images/date_footer.png"
                        alt="calendar"
                        class="check-box pe-1"
                      />
                      <span class="footer-text-color small-font">{{
                        post.date
                      }}</span>
                    </div>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div>
      <div class="debug container-fluid d-flex flex-column align-items-center p-3">
        <div class="d-flex justify-content-center align-items-center pt-2 pb-3 my-gap">
          <div v-for="icona in iconsList" :key="icona.icon" class="d-flex justify-content-center align-items-center bg-orange p-2">
            <img :src="`../../public/images${icona.icon}`" alt="icon">
          </div>
        </div>
        <span class="small-font text-grey py-1">© Fable - Children Kindergarten WordPress Theme by QuanticalLabs</span>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "TheFooter",
  data() {
    return {
      archivesList: [
        {
          date: "October 2014",
          number: 2,
          id: 0,
        },
        {
          date: "September 2014",
          number: 2,
          id: 1,
        },
        {
          date: "August 2014",
          number: 2,
          id: 2,
        },
        {
          date: "July 2014",
          number: 2,
          id: 3,
        },
        {
          date: "June 2014",
          number: 2,
          id: 4,
        },
        {
          date: "May 2014",
          number: 1,
          id: 5,
        },
      ],
      featuresList: [
        {
          text: "Friendly and welcoming place",
        },
        {
          text: "Science and art classes",
        },
        {
          text: "Positive learning enviroment",
        },
        {
          text: "Educational field trips",
        },
        {
          text: "Writing and reading classes",
        },
        {
          text: "Science and art classes",
        },
      ],
      postsList: [
        {
          title: "Drawing and Painting Lessons",
          date: "October 03, 2014",
          img: "/blog_10-150x150.jpg",
        },
        {
          title: "Fall Parents Meeting Day",
          date: "October 03, 2014",
          img: "/blog_09-150x150.jpg",
        },
        {
          title: "Birthday in Kindergarten",
          date: "September 20, 2014",
          img: "/blog_08-150x150.jpg",
        },
      ],
      iconsList: [
        {
          icon: "/behance.png"
        },
        {
          icon: "/dribbble.png"
        },
        {
          icon: "/envato.png"
        },
        {
          icon: "/facebook.png"
        },
        {
          icon: "/twitter.png"
        },
      ]
    };
  },
};
</script>

<style scoped lang="scss">
h4 {
  font-size: 1rem;
}
hr {
  margin-top: 10px;
  width: 26%;
  border: 1px solid white;
  background-color: white;
}
ul {
  list-style: none;
  padding: 0;
}
#logo-footer {
  height: 3.7rem;
}
.small-font {
  font-size: 0.7rem;
}
.medium-font {
  font-size: 0.8rem;
  font-weight: bold;
}
.text-grey {
  color: rgb(168, 168, 168);
}
.debug {
  border: 1px dashed red;
}
.padd {
  padding: 0px 250px;
}
.my-gap {
  gap: 1px;
}
.bg-footer {
  background-image: url("../../public/images/pattern.png");
}
.bg-orange {
  background-color: #fe6500;
}
.footer-text-color {
  color: #a9a6cf;
}
.archive-box {
  border: 1px solid #a9a6cf;
  padding: 9px 6px;
  font-weight: bold;
}
.check-box {
  height: 0.8rem;
}

</style>
