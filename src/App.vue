<template>
  <div>
    <nav-bar/>
    <div id="app" class="">
      <Home id="home"/>
      <Products id="products"/>
      <Testimonials id="testimonials"/>
      <Contact id="contact"/>
    </div>
    <Footer />
  </div>
</template>

<script>
import NavBar from "@/components/NavBar";
import Home from "@/components/Home";
import Products from "@/components/Products";
import Testimonials from "@/components/Testimonials";
import Contact from "@/components/Contact";
import Footer from "@/components/Footer";
export default {
  name: 'App',
  components: {
    NavBar,
    Home,
    Products,
    Testimonials,
    Contact,
    Footer
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
