<template>
  <div class="card">
    <img  v-lazy="pic" class="img">
    <div class="card-content">
      <div class="desc">{{data.desc}}</div>
      <div class="card-content-bottom">
        <div class="who">{{data.who}}</div>
        <div class="time">2017-12-33</div>
      </div>
    </div>
  </div>

</template>

<script>
  export default {
    name: 'v-card',
    props: {
      data: {
        type: Object
      },
      pic: String
    }
  };
</script>
<style lang="stylus" rel="stylesheet/stylus">
  @import "card.styl";
</style>
