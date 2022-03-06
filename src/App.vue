<script>
import Navbar from  './components/nav-bar.vue'
import  MainHome from './components/main-home.vue'
import About from './components/about-us.vue'
import Footer from './components/footer-b.vue'
import FirstSemester from './components/semesters/semester-1.vue'

const routes={
  '/':MainHome,
  '/about': About,
  '/firstsemester':FirstSemester
}

export default{
 name:'app',
  components:{
    Navbar,
    Footer
  },
  data() {
    return {
      currentPath:window.location.hash
    }
  },
  computed:{
    currentView(){
      return routes[this.currentPath.slice(1) || '/'] || About
    }
},
mounted(){
    window.addEventListener('hashchange',()=>{
      this.currentPath=window.location.hash
    })
}
}


</script>

<template>
  <div class="parent">
    <Navbar />
  </div>
   <component :is="currentView" />
   <div>
     <Footer />
   </div>
</template>
<style scoped>
.parent{
  position: fixed;
  top:0;
  left: 0;
  margin:auto;
  width:100%;
  z-index: 3;
  }
</style>
