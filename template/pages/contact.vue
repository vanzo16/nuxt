<template>
  <div>
    <h1>My contacts</h1>
    <p>vanzo16@ya.ru</p>
  </div>
</template>

<script>
export default {
  transition(){
    return 'slide'
  },
  head: {
    title: 'Contact page'
  }
}
</script>

<style>
   h1 {
     font-size: 42px;
   }
   a {
     text-decoration: none;
     font-size: 24px;
     color: #000;
   }

</style>