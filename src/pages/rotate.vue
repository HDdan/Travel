<template>
  <div>
    <img src="../assets/mm.png" alt="" class="Rotation img">
  </div>
</template>

<script>
  // import jquery from 'jquery'
  export default {
    name: "rotate"
  }
  $(function () {
    setTimeout(function () {
      $(".img").addClass("dev");
      $(".img").hide();
    },5000)
  });
</script>

<style scoped>
  img{
    width: 40px;
  }
  .Rotation {
    transform: rotate(360deg);
    animation: rotation 2s linear infinite;
  }
  @keyframes rotation {
    from {-webkit-transform: rotate(0deg);
    }to {
       -webkit-transform: rotate(360deg);
     }
  }
  .dev{
    animation-play-state: paused;
  }
</style>
