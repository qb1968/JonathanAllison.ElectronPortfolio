<template>
  <div class="tweets">
    <a
      class="twitter-timeline"
      :href="src"
      :data-height="420"
      :data-width="350"
      :data-theme="dark ? 'dark' : 'light'"
      :data-link-color="dataLinkColor"
    ></a>
    <a
      class="twitter-timeline"
      :href="src1"
      :data-height="420"
      :data-width="350"
      :data-theme="dark ? 'dark' : 'light'"
      :data-link-color="dataLinkColor"
    ></a>
  </div>
</template>

<script>
export default {
  props: {
    src: {
      type: String,
      default: "https://twitter.com/ethereum?ref_src=twsrc%5Etfw",
    },
    dark: {
      type: Boolean,
      default: false,
    },
    dataLinkColor: {
      type: String,
      default: "#2B7BB9",
    },
    src1: {
      type: String,
      default: "https://twitter.com/BBCAfrica?ref_src=twsrc%5Etfw",
    },
    dark1: {
      type: Boolean,
      default: false,
    },
    dataLinkColor1: {
      type: String,
      default: "#2B7BB9",
    },
  },
  created() {
    let twitterFeed = document.createElement("script");
    twitterFeed.setAttribute("src", "https://platform.twitter.com/widgets.js");
    document.head.appendChild(twitterFeed);
  },
};
</script>

<style>
.tweets {
  display: flex;
  justify-content: space-evenly;
  padding: 10px;
}
</style>
