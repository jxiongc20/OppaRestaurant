<template>
    <nav class="navbar">
    <ul>
      <li><a href="#menu" @click="currentPage = 'menu'">Menu</a></li>
      <li><a href="#home" @click="currentPage = 'home'">Home</a></li>
    </ul>
  </nav>
  <section v-if="currentPage === 'home'" id="home">
      <h1 class="text">Oppa's Kitchen</h1>
   <img src="./assets/OppaLogo.png" class="image" 
   width="300"/>
   <br>
  <h2 class="welcome" style="border: 3px; text-align: center; font-size: 30px;">
    Come hungry, leave happy!
  </h2>
  <br>
  <h3 class="description" style="border: 3px; text-align: center; font-size: 20px;">
    Oppa's Kitchen offers authentic Korean cuisine made with fresh ingredients and traditional recipes. 
    Experience the rich flavors of Korea in every bite! 
  </h3>
  <h3 class="description" style="border: 3px; text-align: center; font-size: 20px;">Join us and taste our delicious cookings straight from the hands of our Oppa.
  </h3>
  </section>

  <section v-if="currentPage === 'menu'" id="menu">
    <h2 class="text" style="border: 3px; text-align: center; font-size: 80px;">Hungry? Oppa got you!</h2>
    <ul>
      <li class="item" style="border: 3px; text-align: center; list-style-type: none; font-size: 30px;">Samgyeopsal - $15.99</li>
      <h3 style="border: 3px; text-align: center; font-size: 20px;">Perfectly seared pork belly wrapped in lettuce</h3>
      <img src="./assets/samgyeopsal.png" class="image" width="120"/>      
      
      <li class="item" style="border: 3px; text-align: center; list-style-type: none; font-size: 30px;">Kimchi Jjigae - $12.99</li>
      <h3 style="border: 3px; text-align: center; font-size: 20px;">Delicious Korean stew with fermented kimchi</h3>
      <img src="./assets/Kimchi Jjiggae.png" class="image" width="120"/>
      
      <li class="item" style="border: 3px; text-align: center; list-style-type: none; font-size: 30px;">Bibimbap - $10.99</li>
      <h3 style="border: 3px; text-align: center; font-size: 20px;">Well balanced Korean rice bowl with vegetables</h3>
      <img src="./assets/bibimbap.png" class="image" width="120"/>
      
      <li class="item" style="border: 3px; text-align: center; list-style-type: none; font-size: 30px;">Tteokbokki - $8.99</li>
      <h3 style="border: 3px; text-align: center; font-size: 20px;">Spicy Korean rice cakes with vegetables</h3>
      <img src="./assets/Tteokbokki.png" class="image" width="120"/>
      
      <li class="item" style="border: 3px; text-align: center; list-style-type: none; font-size: 30px;">Korean Fried Chicken - $15.99</li>
      <h3 style="border: 3px; text-align: center; font-size: 20px;">Crispy and juicy Korean fried chicken in soy garlic & gochujang</h3>
      <img src="./assets/Korean Fried Chicken.png" class="image" width="120"/>
    </ul>
  </section>

  </template>
  <script>
  export default {
    data () {
      return {
        currentPage: "home"
      };
        
      }
    } ;  
</script>
