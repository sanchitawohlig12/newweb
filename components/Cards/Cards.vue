<template>
  <v-container>
    <scroll-wrap target="blog-list">
      <h3 class="display-2 text-center mb-4">Latest News</h3>
      <p class="body-1 text-center mb-4">
        Quis ipsum suspendisse ultrices gravida. Risus commodo viverra maecenas
        accumsan lacus vel facilisis.
      </p>
      <div id="blog-list" class="blog-wrap">
        <v-row justify="center">
          <v-col md="9" cols="12">
            <v-row>
              <v-col
                v-for="(item, index) in blogData"
                :key="index"
                md="4"
                cols="12"
                class="px-4"
              >
                <v-card max-width="500">
                  <v-img :src="item.img" class="white--text" height="200px" />
                  <v-card-title class="title">
                    {{ item.title }}
                  </v-card-title>
                  <v-card-text>
                    <span class="text--primary">
                      <span>{{ item.desc }}</span>
                    </span>
                  </v-card-text>
                  <v-card-actions>
                    <v-btn text color="black"> Read more </v-btn>
                  </v-card-actions>
                </v-card>
              </v-col>
            </v-row>
          </v-col>
        </v-row>
      </div>
    </scroll-wrap>
  </v-container>
</template>

<style scoped lang="scss">
//@import './blog-style';
</style>

<script>
//import BlogCard from '../Cards/BlogCard'
//import ScrollWrap from '../ScrollWrap'

export default {
  components: {
    //BlogCard,
    //ScrollWrap,
  },
  data() {
    return {
      blogData: [
        {
          title: "How to Document Processes to Scale Your Agency",
          desc: "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.",
          img: "https://genial-react.envytheme.com/images/agency-blog1.jpg",
        },
        {
          title: "15 Employee Feedback Tools to Track Your Team",
          desc: "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.",
          img: "https://genial-react.envytheme.com/images/agency-blog2.jpg",
        },
        {
          title: "12 Tried-and-True Ways to Improve User",
          desc: "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.",
          img: "https://genial-react.envytheme.com/images/agency-blog3.jpg",
        },
      ],
    };
  },
};
</script>
<style scoped>
.title {
  font-size: 20px;
  font-weight: bold;
}
</style>
