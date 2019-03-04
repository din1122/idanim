<template>
<div>
<section id="one">
   <Home />
</section>
<section id="two">
<Products />
</section>
<section id="three">
<MoreProducts />
</section>
<section>
<Gallery />
</section>
<section id="four">
<About />
</section>
<section id="fiv">
<Video />
</section>
<section id="six">
<Contact />
</section>
</div>
</template>
<script>
import MoreProducts from '@/components/MoreProducts'
import Products from '@/components/Products'
import Home from '@/components/Home'
import Video from '@/components/Video'
import About from '@/components/About'
import Contact from '@/components/Contact'
import Gallery from '@/components/Gallery'
export default {
   data(){
      return{

      }
   },
   components: {
      Home, Products, MoreProducts,Video, About, Contact, Gallery
  }
}
</script>
