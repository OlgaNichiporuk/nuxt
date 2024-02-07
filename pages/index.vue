<template>
  <div id="main">
    <Game />
    <!-- <div v-for="post in posts">
    <Game :number="post.number" :question="post.question" :answer_1="post.answer_1" :answer_2="post.answer_2" :answer_3="post.answer_3" :answer_4="post.answer_4"></Game>
    </div> -->






  </div>
</template>

<script lang="ts">
import Vue from 'vue'
import Game from '../components/Game.vue';

let posts: [{
  number:"1.",
  question:'В скольких номинациях получил «Оскара» фильм «Титаник»?',
  answer_1: '11',
  answer_2: '10',
  answer_3: '12',
  answer_4: '7',
}]


export default Vue.extend({
  name: 'IndexPage'
})

</script>
<style lang="css">
#main {
  background-image: url('..\image\wallpaper.jpg');
  background-repeat: no-repeat;
  width: 1280px;
  height: 900px;
  padding: 270px;
  padding-top: 10px;
  display: flex;
  align-items: center;

}
</style>