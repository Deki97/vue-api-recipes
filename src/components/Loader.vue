<template>
    <div class="loader">
        <div class="loadingio-spinner-dual-ball-c3azdxir2lu"><div class="ldio-ofa6pjjcmxn">
        <div></div><div></div><div></div>
        </div></div>
    </div>
</template>


<script>
export default {
    name: 'Loader'
}
</script>


<style lang="scss" scoped>
.loader {
    text-align: center;

    @keyframes ldio-ofa6pjjcmxn-o {
    0%    { opacity: 1; transform: translate(0 0) }
   49.99% { opacity: 1; transform: translate(80px,0) }
   50%    { opacity: 0; transform: translate(80px,0) }
  100%    { opacity: 0; transform: translate(0,0) }
}
@keyframes ldio-ofa6pjjcmxn {
    0% { transform: translate(0,0) }
   50% { transform: translate(80px,0) }
  100% { transform: translate(0,0) }
}
.ldio-ofa6pjjcmxn div {
  position: absolute;
  width: 80px;
  height: 80px;
  border-radius: 50%;
  top: 60px;
  left: 20px;
}
.ldio-ofa6pjjcmxn div:nth-child(1) {
  background: #f7972e;
  animation: ldio-ofa6pjjcmxn 1s linear infinite;
  animation-delay: -0.5s;
}
.ldio-ofa6pjjcmxn div:nth-child(2) {
  background: #7b69a2;
  animation: ldio-ofa6pjjcmxn 1s linear infinite;
  animation-delay: 0s;
}
.ldio-ofa6pjjcmxn div:nth-child(3) {
  background: #f7972e;
  animation: ldio-ofa6pjjcmxn-o 1s linear infinite;
  animation-delay: -0.5s;
}
.loadingio-spinner-dual-ball-c3azdxir2lu {
  width: 200px;
  height: 200px;
  display: inline-block;
  overflow: hidden;
  background: #ffffff;
}
.ldio-ofa6pjjcmxn {
  width: 100%;
  height: 100%;
  position: relative;
  transform: translateZ(0) scale(1);
  backface-visibility: hidden;
  transform-origin: 0 0;
}
.ldio-ofa6pjjcmxn div { box-sizing: content-box; }
}
</style>