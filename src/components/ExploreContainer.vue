<template>
  <div id="container">
    <img src="../../resources/R-C.png" alt="">

    <p>欢迎使用懒猫相册！</p>
    <p>请开启相册权限享用更多功能。</p>
    
    <ion-button 
      shape="round" 
      color="tertiary"
    >
      开启相册权限
    </ion-button>

  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue';

export default defineComponent({
  name: 'ExploreContainer',
  props: {
    name: String
  }
});
</script>

<style scoped>
img {
  max-width: 50%;
  margin-bottom: 20px;
}
ion-button {
  margin-top: 20px;
}
#container {
  text-align: center;
  position: absolute;
  left: 0;
  right: 0;
  top: 50%;
  transform: translateY(-50%);
}

#container strong {
  font-size: 20px;
  line-height: 26px;
}

#container p {
  font-size: 16px;
  line-height: 22px;
  color: #8c8c8c;
  margin: 0;
}

#container a {
  text-decoration: none;
}
</style>
