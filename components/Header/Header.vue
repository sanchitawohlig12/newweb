<!--template>
  <div class="head">
    <!-- :class="{ 'mobile': $vuetify.breakpoint.smAndDown, 'head': $vuetify.breakpoint.smAndUp}"  -->
    <!--h1 class="mobile">
      {{ title }}
    </!--h1>
    <p class="mobile">Let's Travel Together</p>
  </div>
</!--template>

<!--script>
export default {
  data() {
    return {
      title: "Welcome",
    };
  },
};
</!--script>

<!--style>
.head {
  text-align: center;
}
</!--style!-->

<template>
  <div>
    <v-carousel cycle :height="$vuetify.breakpoint.smAndUp ? '600' : '600'">
      <v-carousel-item
        v-for="(item, i) in items"
        :key="i"
        :src="item.src"
        reverse-transition="fade-transition"
        transition="fade-transition"
        justify="center"
      >
        <h1 align="center" class="h1">
          {{ item.title }}
        </h1>
        <h3 class="p">
          {{ item.caption }}
        </h3>
        <v-btn class="btn" x-large rounded color="primary" dark align="center">
          Get Started
        </v-btn></v-carousel-item
      >
    </v-carousel>
  </div>
</template>
<script>
export default {
  data() {
    return {
      items: [
        {
          src: "https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTvQOfYdk20E70vc5D1tV34WwC5jSSP3oEpLQ&usqp=CAU.jpg",
          title: "Ultimate Platform to monitor your best workflow.",
          caption:
            "It should be noted that although application software is thought of asa program, it can be anything that runs on a computer.",
        },
        {
          src: "https://image.shutterstock.com/image-photo/leaves-dark-shade-600w-1065614543.jpg",
          title: "Ultimate Platform to monitor your best workflow.",
          caption:
            "It should be noted that although application software is thought of asa program, it can be anything that runs on a computer.",
        },
        {
          src: "https://image.shutterstock.com/image-photo/leaves-dark-shade-600w-1065614543.jpg",
          title: "Ultimate Platform to monitor your best workflow.",
          caption:
            "It should be noted that although application software is thought of asa program, it can be anything that runs on a computer.",
        },
        {
          src: "https://wallpaperaccess.com/full/2957951.jpg",
          title: "Ultimate Platform to monitor your best workflow.",
          caption:
            "It should be noted that although application software is thought of asa program, it can be anything that runs on a computer.",
        },
      ],
    };
  },
};
</script>
<style scoped>
.h1 {
  color: white;
  margin-top: 100px;
}
.p {
  color: white;
  font-size: 25px;
  text-align: center;
}
.btn {
  size: 50px;
  align-content: center;
  margin-left: 450px;
  margin-top: 100px;
}
</style>