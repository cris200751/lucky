<template>
  <div class="social-network-con">
    <ul class="list-social-network">
      <li @click="jumpclick('https://t.me/luckymetaverse')">
        <img class="nohover" src="../../../static/images/Telegram_logo.png" />
        <img class="hover" src="../../../static/images/Telegram_logoyes.png" />
      </li>
      <li @click="jumpclick('https://discord.gg/JTstQ8Tm')">
        <img class="nohover" src="../../../static/images/happyicon.png" />
        <img class="hover" src="../../../static/images/happyiconyes.png" />
      </li>
      <li
        @click="jumpclick('https://www.facebook.com/LuckyMeta-102656795685121')"
      >
        <img class="nohover" src="../../../static/images/fbicon.png" />
        <img class="hover" src="../../../static/images/fbiconyes.png" />
      </li>
      <li @click="jumpclick('https://twitter.com/LuckyMetaverse')">
        <img class="nohover" src="../../../static/images/twittericon.png" />
        <img class="hover" src="../../../static/images/twittericonyes.png" />
      </li>
      <li
        @click="
          jumpclick('https://www.youtube.com/channel/UCl66czQcUxBU-iZ9yYjBclA')
        "
      >
        <img class="nohover" src="../../../static/images/YouTube.png" />
        <img class="hover" src="../../../static/images/YouTubeyes.png" />
      </li>
    </ul>
  </div>
</template>
<script>
export default {
  methods: {
    jumpclick(url) {
      window.open(url, "_blank");
    },
  },
};
</script>
<style scoped>
.social-network-con {
  width: 700px;
  margin: auto;
  margin-top: 20px;
}

.list-social-network {
  display: flex;
}

.list-social-network li {
  flex-grow: 1;
  text-align: center;
}

.list-social-network li img {
  margin: auto;
}

.list-social-network li .hover {
  display: none;
}

.list-social-network li:hover .hover {
  display: block;
}

.list-social-network li:hover .nohover {
  display: none;
}
</style>