<template>
<div>
  <div>
    <img class="pic" src="./assets/vue1.jpg" alt="vue1">
    <p>책 제목 : vue.js 1 </p>
    <!-- vue 문법 {{}} = 변수값 가져옴-->
    <p>저자    : {{author1}} </p> 
    <p>가격    : {{prices[0]}} </p> 
  </div>
  <div>
    <img class="pic" src="./assets/vue2.jpg" alt="vue2">
    <p>책 제목 : vue.js 2 </p>
    <p>저자    : {{author2}} </p> 
    <p>가격    : {{prices[1]}} </p> 
  </div>
  <div>
    <img class="pic" src="./assets/vue3.jpg" alt="vue3">
    <p>책 제목 : vue.js 3 </p>
    <p>저자    : {{author3}} </p> 
    <p>가격    : {{prices[2]}} </p> 
  </div>

</div>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'

export default {
  name: 'App',
  components: {//내용을 써주지 않으면 생략해도 된다.
  },
  data() {
    return {
      author1 : "임꺽정",
      author2 : "홍길동2",
      author3 : "홍길동3",
      prices  : [15000,25000,30000]
    }
  }
}
</script>

<style>
  .pic {
    width: 200px;
    border: 1px solid orange;
  }
</style>
