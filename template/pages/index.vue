<template>
  <div>
    <h1>Welcome!</h1>
  </div>
</template>

<script>
export default {
  transition(){
    return 'slide'
  },
  head: {
    title: 'Home page'
  }
}
</script>

<style>
   h1 {
     font-size: 42px;
   }
  

</style>




import {TimelineMax} from 'gsap';

export default {
  transition: {
    name: 'test',
    mode: 'out-in',
    css: false,
    enter: function(el, done){
      let tl = new TimelineMax({onComplete: done});
      tl.fromTo(el, 0.3, {y:-100, opacity:0, rotation:30},{y:0, opacity:1, rotation:0})
    },
    leave: function(el, done){
      let tl = new TimelineMax({onComplete: done});
      tl.fromTo(el, 0.3, {y:0, opacity:1},{y:100, opacity:0})
    }
  },

}