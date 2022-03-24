<template>
<TheNavbar />
 <div>
    <TheHeader/>
    <main>
      <p>Find gorgeous spots to visit this summer by simply searching for them on our website.</p>
      </main>
    <SearchForm/>
  </div>
  <caption-content>
    <template #content>
      <img 
      src="https://images.pexels.com/photos/846265/pexels-photo-846265.jpeg?cs=srgb&dl=pexels-the-happiest-face-%29-846265.jpg&fm=jpg"
      />
      <TicketPrice />
    </template>
    <template #caption="{source}">
     Image Source: <a href="pexels.com">{{source}}</a>
    </template>
  </caption-content>
      <TheFooter />
      <template>
    <footer>
     <p>&copy;Jibril Adem</p>
    </footer>
</template>
      
</template>

<script>

import CaptionContent from  './components/CaptionContent.vue'
import TheFooter from './components/TheFooter.vue'
import TheHeader from './components/TheHeader.vue'
import TheNavbar from './components/TheNavbar.vue'
import SearchForm from './components/SearchForm.vue'
import TicketPrice from './components/TicketPrice.vue'

export default {
  components: {
    CaptionContent,
    TheFooter,
    TheHeader,
    TheNavbar,
    SearchForm,
    TicketPrice,
  },
}
</script>
<style>

#app {

  font-family: Arial, Helvetica, sans-serif;
  text-align: center;
  color: red;
  background: black;
}

</style>