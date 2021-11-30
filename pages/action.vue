<template>
  <div class="container">
    <div class="changesuru">
      {{ text }}{{ text2 }}
    </div>
    <button @click="changeTextTry()">{{ btnNameCange }}</button>
    <button @click="changeTextDefault()">{{ btnNameDefault }}</button>
    <hr>
    <router-link to="/">Topページへのリンクです</router-link>
    <hr>
    <router-link to="/hello">Helloページへのリンクです</router-link>
    <hr>
    <router-link to="/input">Inputページへのリンクです</router-link>
    <hr>
  </div>
</template>
 
<script lang="ts">
import Vue from 'vue'
 
export default Vue.extend({
  data: () => ({
    text: '文字を',
    text2: '変更しますか？',
    btnNameCange: '文字を変更変更しました！にするボタン',
    btnNameDefault:'文字を変更しますか？にするボタン',
  }),
  methods: {
    changeTextTry() {
      this.text2 = '変更しました！'
    },
    changeTextDefault() {
      this.text2 = '変更しますか？'
    },
  },
})
</script>
 
<style></style>