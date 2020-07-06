<template>
  <div class="review-card">
    <div>
      <span class="size-15 white">{{review}}</span>
    </div>
    <div id="review-card-user">
      <div>
        <img class="avatar" :src="getImgUrl(avatar)" alt="avatar" />
      </div>
      <div>
        <span class="size-15 white bold">{{name}}</span>
        <br />
        <span class="size-15 white">{{position}}</span>
      </div>
    </div>
  </div>
</template>

<script>
import data from "../data";

export default {
  props: ["avatar", "name", "position", "review"],
  methods: {
    getImgUrl(name) {
      var images = require.context("../assets/images", false, /\.jpg$/);
      return images("./" + name + ".jpg");
    }
  }
};
</script>


<style>
.review-card {
  width: 300px;
  background-color: hsl(219, 30%, 18%);
  border-radius: 5px;
  padding: 30px 20px 20px 20px;
  cursor: pointer;
  transition: all 0.3s;
  -webkit-box-shadow: -1px 3px 5px 0px rgba(0, 0, 0, 0.39);
  -moz-box-shadow: -1px 3px 5px 0px rgba(0, 0, 0, 0.39);
  box-shadow: -1px 3px 5px 0px rgba(0, 0, 0, 0.39);
}

#review-card-user {
  display: flex;
  flex-direction: row;
  margin-top: 12px;
}

.review-card:hover {
  transform: scale(1.04);
}
</style>

