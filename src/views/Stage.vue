<template>
  <div class="stage">
    <!-- <a href="#" class="glitch"></a> -->
  </div>
</template>

<script>
// @ is an alias to /src
</script>

<style lang="scss" scoped>
  .glitch {
  font-size: 130px;
  line-height: 1;
  font-family: 'Poppins', sans-serif;
  font-weight: 700;
  position:absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  margin: 0;
  text-decoration: none;
  color: #fff;
  &:before,
  &:after{
    display: block;
    content: '1';
    position: absolute;
    top: 0;
    left: 0;
    height: 100%;
    width: 100%;
    opacity: .8;
  }
  &:after {
    color: #f0f;
    z-index: -2;
  }
  &:before {
    color: #111;
    z-index: -1;
  }
  &:hover {
    &:before {
      animation: glitch .6s cubic-bezier(.25, .46, .45, .94) both infinite
    }
    &:after {
      animation: glitch .6s cubic-bezier(.25, .46, .45, .94) reverse both infinite
    }
  }
}
@keyframes glitch {
    0% {
        -webkit-transform: translate(0);
        transform: translate(0)
    }
    20% {
        -webkit-transform: translate(-3px, 3px);
        transform: translate(-3px, 3px)
    }
    40% {
        -webkit-transform: translate(-5px, -5px);
        transform: translate(-5px, -5px)
    }
    60% {
        -webkit-transform: translate(5px, 5px);
        transform: translate(5px, 5px)
    }
    80% {
        -webkit-transform: translate(5px, -5px);
        transform: translate(5px, -5px)
    }
    to {
        -webkit-transform: translate(0);
        transform: translate(0)
    }
}
</style>
