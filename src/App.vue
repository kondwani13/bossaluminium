<template>

<nav class="sticky overflow-x-hidden top-0 opacity-80 font-sans items-center inline-flex  py-1  lg:pl-40  bg-gray-900 shadow w-full z-40">

  <div class="pl-6 lg:pl-10">
    <a @click="scrollToAnchorPoint('home')" class=" "><img class=" w-8" src="https://i.postimg.cc/Wby05tXK/blogo.png" alt="logos"></a>
    
  </div>
  
  <div class="pl-10 pr-3 lg:pl-96 inline-flex">
    
    <button @click="scrollToAnchorPoint('clients')" class="text-sm lg:text-lg no-underline text-indigo-300 hover:text-white px-2 lg:px-4 ">clients</button>
    
    
    <button @click="scrollToAnchorPoint('services')" class="peer text-sm lg:text-lg no-underline text-indigo-300 hover:text-white px-2 lg:px-4">services</button>
        
       

    <button @click="scrollToAnchorPoint('about')" class="text-sm lg:text-lg no-underline text-indigo-300 hover:text-white px-2 lg:px-4">about</button>
    <button @click="scrollToAnchorPoint('reach')" class="hidden lg:block text-sm lg:text-lg no-underline text-indigo-300 hover:text-white px-2 lg:px-4">contacts</button>
    <button @click="scrollToAnchorPoint('faq')" class="text-sm lg:text-lg no-underline text-indigo-300 hover:text-white px-2 lg:px-4">faq</button>
    <a href="https://wa.me/260975777778" ><img class="w-5 mt-1 ml-2 " src="https://i.ibb.co/JzHhXJn/app.png" alt="cw"></a>
    
    
	
		
	
  </div>

  
    
</nav>
	
 <div ref="home" class="w-full bg-cover bg-center -mt-24">
       
     <div class="bg-white font-sans leading-normal tracking-normal">

<div class="carousel relative shadow-2xl bg-white">
  <div class="carousel-inner relative overflow-hidden w-full">
    <!--Slide 1-->
    <input class="carousel-open" type="radio" id="carousel-1" name="carousel" aria-hidden="true" hidden="" checked="checked">
    <div class="carousel-item absolute opacity-0" style="">
      <div class=" text-white text-5xl text-center"><img class="w-full bg-cover bg-center" src="https://i.postimg.cc/xTpKjMds/h2.jpg" alt="h2"></div>
    </div>
    <label for="carousel-3" class="prev control-1 w-10 h-10 ml-2 md:ml-10 absolute cursor-pointer hidden text-3xl font-bold text-black hover:text-white rounded-full bg-white opacity-10 hover:bg-blue-700 leading-tight text-center z-10 inset-y-0 left-0 my-auto">‹</label>
    <label for="carousel-2" class="next control-1 w-10 h-10 mr-2 md:mr-10 absolute cursor-pointer hidden text-3xl font-bold text-black hover:text-white rounded-full bg-white opacity-10 hover:bg-blue-700 leading-tight text-center z-10 inset-y-0 right-0 my-auto">›</label>
    
    <!--Slide 2-->
    <input class="carousel-open" type="radio" id="carousel-2" name="carousel" aria-hidden="true" hidden="">
    <div class="carousel-item absolute opacity-0" style="">
      <div class=" text-white text-5xl text-center"><img class="w-full bg-cover bg-center" src="https://i.postimg.cc/hjKn5JVn/h1.jpg" alt="h1"></div>
    </div>
    <label for="carousel-1" class="prev control-2 w-10 h-10 ml-2 md:ml-10 absolute cursor-pointer hidden text-3xl font-bold text-black hover:text-white rounded-full bg-white opacity-10 hover:bg-blue-700 leading-tight text-center z-10 inset-y-0 left-0 my-auto">‹</label>
    <label for="carousel-3" class="next control-2 w-10 h-10 mr-2 md:mr-10 absolute cursor-pointer hidden text-3xl font-bold text-black hover:text-white rounded-full bg-white opacity-10 hover:bg-blue-700 leading-tight text-center z-10 inset-y-0 right-0 my-auto">›</label> 
    
    <!--Slide 3-->
    <input class="carousel-open" type="radio" id="carousel-3" name="carousel" aria-hidden="true" hidden="">
    <div class="carousel-item absolute opacity-0" style="">
      <div class=" text-white text-5xl text-center"><img class="w-full bg-cover bg-center" src="https://i.postimg.cc/VLPNqNVY/h3.jpg" alt="h3"></div>
    </div>
    <label for="carousel-2" class="prev control-3 w-10 h-10 ml-2 md:ml-10 absolute cursor-pointer hidden text-3xl font-bold text-black hover:text-white rounded-full bg-white opacity-10 hover:bg-blue-700 leading-tight text-center z-10 inset-y-0 left-0 my-auto">‹</label>
    <label for="carousel-1" class="next control-3 w-10 h-10 mr-2 md:mr-10 absolute cursor-pointer hidden text-3xl font-bold text-black hover:text-white rounded-full bg-white opacity-10 hover:bg-blue-700 leading-tight text-center z-10 inset-y-0 right-0 my-auto">›</label>

    <!-- Add additional indicators for each slide-->
    <ol class="carousel-indicators">
      <li class="inline-block mr-3">
        <label for="carousel-1" class="carousel-bullet cursor-pointer block text-4xl text-white hover:text-blue-700">•</label>
      </li>
      <li class="inline-block mr-3">
        <label for="carousel-2" class="carousel-bullet cursor-pointer block text-4xl text-white hover:text-blue-700">•</label>
      </li>
      <li class="inline-block mr-3">
        <label for="carousel-3" class="carousel-bullet cursor-pointer block text-4xl text-white hover:text-blue-700">•</label>
      </li>
    </ol>


    
  </div>
</div>
</div>  
       

      
    </div>
    <div class="flex justify-center bg-white p-4"><img class="justify-center w-48 lg:w-auto" src="https://i.ibb.co/7V6cjZJ/logo2.png" alt="p1"></div>
    <div class="justify-center overflow-x-hidden   bg-blue-back1 w-full inline-flex pb-4 pt-10 px-4  lg:space-x-36 ">
      <div class="pl-5">
        <img class="w-[40px] lg:w-auto ml-2" src="https://i.postimg.cc/MGjKR58Z/p1.png" alt="p1">
       
      <button  @click="activeTab = 'Odd'" class="text-sm lg:text-2xl text-indigo-300 hover:text-white pr-5 lg:pr-0 ">Total projects</button>
      </div>
      <div class="pl-5">
        <img class="w-[40px] lg:w-auto ml-2 " src="https://i.postimg.cc/htYtfw63/s1.png" alt="p1">
        
       <button  @click="activeTab = 'Lucky'" class="text-sm lg:text-2xl text-indigo-300 hover:text-white pr-5 lg:pr-0 ">Staff members</button>
      </div>
      <div class="pl-5">
        <img class="w-[40px] lg:w-auto ml-1 " src="https://i.postimg.cc/qMjRdgLr/t1.png" alt="p1">
        
       <button  @click="activeTab = 'Niu'" class="text-sm lg:text-2xl text-indigo-300 hover:text-white pr-5 lg:pr-0 ">Hours of work</button>
      </div>
      <div class="pl-5">
        <img class="w-[40px] lg:w-auto " src="https://i.postimg.cc/vZTm8MqV/l1.png" alt="p1">
        
       <button  @click="activeTab = 'Equal'" class="text-sm lg:text-2xl text-indigo-300 hover:text-white pr-5 lg:pr-0 ">Major cities</button>
       </div>
        
    </div>
   <div class="bg-blue-back1 lg:pb-0 pb-8 pt-2 lg:pt-12  lg:px-52">

   


    
       

       <div class=""> <component :is="activeTab" /></div>
       
         


  </div>


 <div class="overflow-hidden pt-2 lg:pt-12  lg:px-52">
        <div class="mx-4 md:mx-12 py-3 lg:py-8 md:py-12 grid place-content-center px-4 md:px-0">
            <div class="lg:flex justify-start lg:gap-28">

                <div class="pt-8 lg:pt-0">
                    <img src="https://i.ibb.co/3ffjs38/vrbg.png" alt="man in black suit holding brown paper" class="hidden lg:block" />
                    <img src="https://i.ibb.co/3ffjs38/vrbg.png" alt="man in black suit holding brown paper" class="hidden sm:block lg:hidden" />
                    <img src="https://i.ibb.co/02DzWv4/vrsm.png" alt="man in black suit holding brown paper" class="sm:hidden" />
                </div>

                <div class="lg:mt-6 lg:pt-3">
                    <h1 class="font-bold text-3x1 lg:text-5xl text-black text-left">Visit our Showroom</h1>
                    <p class="pt-3 lg:pt-8 md:pt-4 text-gray-700 text-left">Take a look at our online virtual showroom where we showcase some of our modern designs and have a feel of boss aluminum</p>
                    
                    <button class="relative px-6 py-2 group mt-5 lg:mt-10">
                    <span class="absolute inset-0 w-full h-full transition duration-200 ease-out transform translate-x-1 translate-y-1 bg-indigo-700 group-hover:-translate-x-0 group-hover:-translate-y-0"></span>
                    <span class="absolute inset-0 w-full h-full bg-white border-2 border-indigo-700 group-hover:bg-indigo-700"></span>
                    <span class="relative text-indigo-700 group-hover:text-indigo-100"><a href="https://stupendous-caramel-cdf0e1.netlify.app/"> Let's go</a> </span>
                    </button>
                </div>
                
            </div>
        </div>
    </div>
      

     <div ref="services" class="">
     <h4 class="text-white lg:text-5xl text-2xl font-bold text-center bg-blue-imb lg:py-20  py-8">Our services</h4>
    

      <div class="flex items-center justify-center px-4 pt-4 lg:px-16 lg:py-12 bg-white w-full inline-flex  space-x-2 lg:space-x-44  ">
      

      <div class=""><button @click="Live = 'Aluminium'"> <img class="pl-4 w-48" src="https://i.ibb.co/Kwx7Lbh/ba.png" alt="sym1">
      
      </button>
      </div>
      <div class=""><button @click="Live = 'Wood'"><img class="pl-4 w-48" src="https://i.ibb.co/MNHWzTc/bw.png" alt="sym2">
      
      </button>
      </div>
      <div class=""><button @click="Live = 'Glass'"><img class="pl-4 w-48" src="https://i.ibb.co/vYBkV60/bg.png" alt="sym3">
      
      </button>
      </div>
      </div>
      </div>
      <div class="lg:hidden bg-white p-6"><component :is="Live" /></div>

      <div class="flex items-center justify-center bg-white pb-8">
      <div class="px-44 grid lg:grid-cols-3 lg:grid-flow-row bg-white lg:space-x-8 ">
      <div class="px-6 py-8 hidden md:block rounded-lg bg-blue-imbt hover:bg-blue-hov hover:text-white">
      
      
      <p class="text-blue-textm hover:text-white text-base  "><span class="font-semibold text-2xl pb-4">Aluminium</span></p>
      <p class=" text-blue-textm text-base py-3">We provide 3 profiles, the European, South African and Middle East profile.</p>
     
     <ul class=" list-disc marker:text-blue-500 text-base text-blue-textm hover:text-white text-base pl-5">
        <LI>Aluminium windows</LI>
        <li>Aluminium doors</li>
        <li>Aluminium enclosures</li>
        
        <li>Folding doors</li>
        <li>Shop fronts</li>
        <li>Aluminium partitions</li>
     </ul>
     
      
       </div>
       <div class="px-6 py-8 hidden md:block rounded-lg bg-blue-imbt hover:bg-blue-hov hover:text-white">
      
      
      <p class="text-blue-textm hover:text-white text-base  "><span class="font-semibold text-2xl pb-4">Wood</span></p>
     
     
     <ul class="list-disc marker:text-blue-500 text-base text-blue-textm hover:text-white text-base pl-5">
        <LI>Kitchen units</LI>
        <li>Doors </li>
        <li>Ceiling boards</li>
        
        <li>Wardrobes</li>
        <li>Repairs & Remodeling</li>
        
      
     </ul>
     
      
       </div>
       <div class="px-6 py-8 hidden md:block rounded-lg bg-blue-imbt hover:bg-blue-hov hover:text-white">
      
      
      <p class="text-blue-textm hover:text-white text-base  "><span class="font-semibold text-2xl pb-4">Glass</span></p>
      
     
    <ul class="list-disc marker:text-blue-500 text-base text-blue-textm hover:text-white text-base pl-5">
        <LI>Glass partitions</LI>
        <li>Glass cutting</li>
        <li>Table top</li>
        
        <li>Shower enclosures</li>
        <li>Mirrors</li>
        <li>Window Vinyl Frosting</li>
        <li>Flush glazing</li>
     </ul>
     
      
       </div>

      </div>
      </div>
   


      
       <div class="lg:p-8 p-4 overflow-x-hidden">
        <LightBox />
        </div>
        <div ref="clients" class="">
        <clients />
        </div>
        <div ref="about" class="">
        <about />
        <div ref="reach" class="px-24 hidden lg:block">
          <reach />
        </div>
        </div>
        <div ref="faq" class="">
        <faq />
        </div>


        
<footer class="hidden lg:block lg:px-24 bg-gray-200 rounded-lg shadow md:px-6 md:py-8 dark:bg-gray-900">
    <div class="sm:flex sm:items-center sm:justify-between">
        <a href="https://flowbite.com/" class="flex items-center mb-4 sm:mb-0">
            <img src="https://i.ibb.co/7V6cjZJ/logo2.png" class="mr-3 h-8" alt="Flowbite Logo">
            <span class="self-center text-2xl font-semibold whitespace-nowrap dark:text-white"></span>
        </a>
        <ul class="flex space-x-8 flex-wrap items-center mb-6 text-sm text-gray-500 sm:mb-0 dark:text-gray-400">
            <li>
                <a href="https://web.facebook.com/BOSS-WOOD-105948045363463" ><img class="w-8" src="https://i.postimg.cc/hvYL8SwN/face.png" alt="cw"></a>
            </li>
            <li>
                <button ><img class="w-8" src="https://i.postimg.cc/y6pyCPdn/insta.png" alt="cw"></button>
            </li>
            <li>
                <button ><img class="w-8" src="https://i.postimg.cc/j5ZQ56hx/pin.png" alt="cw"></button>
            </li>
            <li>
                <button @click.prevent="showModal"  class="hover:underline"><img class="w-8" src="https://i.postimg.cc/zDtg6GBg/email.png" alt="cw"></button>
            </li>
        </ul>
    </div>
    <hr class="my-6 border-gray-200 sm:mx-auto dark:border-gray-700 lg:my-8">
    <span class="block text-sm text-gray-500 sm:text-center dark:text-gray-400">© 2022 Boss Aluminium. All Rights Reserved.
    </span>
</footer>
<div class="lg:hidden">
<hr class="my-6 border-gray-200 sm:mx-auto dark:border-gray-700 lg:my-8">
    <span class="flex justify-center p-4 text-sm text-gray-500 sm:text-center dark:text-gray-400">© 2022 Boss Aluminium. All Rights Reserved.
    </span>
    </div>



        
    

    


 

















 <div class="bg-blue-foot sticky bottom-0 lg:hidden z-40 pb-0 overflow-x-hidden overflow-y-0 ">
 <footer class="h-5 mb-3 px-4 pb-6 pt-5 flex inline-flex rounded-t-lg bg-blue-foot w-full items-center text-center space-x-16  justify-center">

    <div class="h-1 pb-4"><a href="https://web.facebook.com/BOSS-WOOD-105948045363463" ><img class="w-8" src="https://i.postimg.cc/hvYL8SwN/face.png" alt="home"></a></div>
    <div class="h-1 pb-4"><button ><img class="w-8" src="https://i.postimg.cc/y6pyCPdn/insta.png" alt="dsign"></button></div>
    <div class="h-1 pb-4"><button ><img class="w-8" src="https://i.postimg.cc/j5ZQ56hx/pin.png" alt="cw"></button></div>
    <div class="h-1 pb-4"><button @click.prevent="showModal"><img class="w-8" src="https://i.postimg.cc/zDtg6GBg/email.png" alt="cw"></button></div>
 </footer>
 </div>
        
     
    
   

    <the-modal-component v-show="isModalVisible"
      @close="closeModal" />

  


</template>


<script>

import TheModalComponent from './components/TheModalComponent.vue';
import Odd from './components/Odd.vue';
import Niu from './components/Niu.vue';
import Lucky from './components/Lucky.vue';
import Equal from './components/Equal.vue';
import Register from './components/Register.vue';
import Purchase from './components/Purchase.vue';
import Transfer from './components/Transfer.vue';
import Automatic from './components/Automatic.vue';
import Aluminium from './components/Aluminium.vue';
import Wood from './components/Wood.vue';
import Glass from './components/Glass.vue';
import Clients from './components/Clients.vue';
import Faq from './components/Faq.vue';
import About from './components/About.vue';
import Contacts from './components/Contacts.vue';
import LightBox from "./components/Lightbox.vue";
import Reach from "./components/Reach.vue";








export default {
    name: 'App',
    components: {
      
      TheModalComponent,
      Contacts,
      LightBox,
      Reach,
      Odd,
      Niu,
      Lucky,
      Equal,
      Register,
      Purchase,
      Transfer,
      Automatic,
      Aluminium,
      Wood,
      Glass,
      Clients,
      Faq,
      About,
      
      

  
    },
   
     data() {
      return {
        isModalVisible: false,
        activeTab: "Odd",
        Tab: "Register",
        open: false,
        Live: Aluminium,
        
       
        
      };
    },
    methods: {
     
      showModal() {
        this.isModalVisible = true;
      },
      closeModal() {
        this.isModalVisible = false;
      },
      scrollToAnchorPoint(refName) {
            const el = this.$refs[refName]
            el.scrollIntoView({ behavior: 'smooth'})
        }
        
    },
   
    
   

}  
</script>
<style scoped>
			.carousel-open:checked + .carousel-item {
				position: static;
				opacity: 100;
			}
			.carousel-item {
				-webkit-transition: opacity 0.6s ease-out;
				transition: opacity 0.6s ease-out;
			}
			#carousel-1:checked ~ .control-1,
			#carousel-2:checked ~ .control-2,
			#carousel-3:checked ~ .control-3 {
				display: block;
			}
			.carousel-indicators {
				list-style: none;
				margin: 0;
				padding: 0;
				position: absolute;
				bottom: 2%;
				left: 0;
				right: 0;
				text-align: center;
				z-index: 10;
			}
			#carousel-1:checked ~ .control-1 ~ .carousel-indicators li:nth-child(1) .carousel-bullet,
			#carousel-2:checked ~ .control-2 ~ .carousel-indicators li:nth-child(2) .carousel-bullet,
			#carousel-3:checked ~ .control-3 ~ .carousel-indicators li:nth-child(3) .carousel-bullet {
				color: #2b6cb0;  /*Set to match the Tailwind colour you want the active one to be */
			}

   
		</style>


