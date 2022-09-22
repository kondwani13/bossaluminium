<template>
    
        <div class="h-80 pb-8">
        <div class="bg-gray-200  rounded-lg z-50  pt-6 shadow-lg w-96 fixed top-1/2 left-1/2 transform -translate-x-1/2 -translate-y-1/2">
         
         
         
        
              
              <div class="xl:w-3/5 lg:w-3/5  bg-gray-200 h-full pb-5 xl:pr-5 xl:pl-0 rounded-tr rounded-br">
               <div class="pl-7">
                    <button @click="close" type="button" class="bg-white rounded-md p-2 items-right justify-right text-gray-400 hover:text-gray-500 hover:bg-gray-100 focus:outline-none focus:ring-2 focus:ring-inset focus:ring-indigo-500">
                    <span class="sr-only">Close menu</span>
                    <!-- Heroicon name: outline/x -->
                    <svg class="h-6 w-6" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke="currentColor" aria-hidden="true">
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M6 18L18 6M6 6l12 12" />
              </svg>
            </button>
            </div>
                <form ref="form" @submit.prevent="sendEmail" class="bg-white py-4 px-8 rounded-tr rounded-br">

                   

                    <h1 class="text-4xl text-gray-800 font-extrabold mb-6">Enter Details</h1>
                    <div class="block xl:flex w-full flex-wrap justify-between mb-6">
                        <div class="w-2/4 max-w-xs mb-6 xl:mb-0">
                            <div class="flex flex-col">
                                <label for="full_name" class="text-gray-800 text-sm font-semibold leading-tight tracking-normal mb-2">Full Name</label>
                                <input required id="full_name" name="full_name" type="text" class="focus:outline-none focus:border focus:border-indigo-700 font-normal w-64 h-10 flex items-center pl-3 text-sm border-gray-300 rounded border" placeholder="" />
                            </div>
                        </div>
                        <div class="w-2/4 max-w-xs xl:flex xl:justify-end">
                            <div class="flex flex-col">
                                <label for="email" class="text-gray-800 text-sm font-semibold leading-tight tracking-normal mb-2">Email</label>
                                <input required id="email" name="email" type="email" class="focus:outline-none focus:border focus:border-indigo-700 font-normal w-64 h-10 flex items-center pl-3 text-sm border-gray-300 rounded border" placeholder="" />
                            </div>
                        </div>
                    </div>
                    <div class="flex w-full flex-wrap">
                        <div class="w-2/4 max-w-xs">
                            <div class="flex flex-col">
                                <label for="phone" class="text-gray-800 text-sm font-semibold leading-tight tracking-normal mb-2">Phone</label>
                                <input required id="phone" name="phone" type="tel" class="focus:outline-none focus:border focus:border-indigo-700 font-normal w-64 h-10 flex items-center pl-3 text-sm border-gray-300 rounded border" placeholder="" />
                            </div>
                        </div>
                    </div>
                    <div class="w-full mt-6">
                        <div class="flex flex-col">
                            <label class="text-sm font-semibold text-gray-800 mb-2" for="message">Message</label>
                            <textarea placeholder="" name="message" class="border-gray-300 border mb-4 rounded py-2 text-sm outline-none resize-none px-3 focus:border focus:border-indigo-700" rows="8" id="message"></textarea>
                        </div>
                        <button type="submit" class="focus:outline-none bg-indigo-700 transition duration-150 ease-in-out hover:bg-indigo-600 rounded text-white px-8 py-3 text-sm leading-6">Submit</button>
                    </div>
                </form>
            </div>

              
           
        </div>
        </div>
    
</template>

<script>

import emailjs from '@emailjs/browser';
export default {
     name: 'TheModalComponent',
    methods: {
         sendEmail() {
      emailjs.sendForm('service_7xaz4fs', 'template_rgmmd4f', this.$refs.form, 'Mfe4USnZ1GPrkngT5')
        .then((result) => {
            console.log('SUCCESS!', result.text);
        }, (error) => {
            console.log('FAILED...', error.text);
        },
        );
         },
      close() {
        this.$emit('close');
      },
    },
  };
    

</script>

<style scoped>
.bounce-enter-active {
    animation: bounce-in .5s ease-out both;
}

.bounce-leave-active {
    animation: bounce-in .5s reverse ease-in both;
}

@keyframes bounce-in {
    0% {
        transform: scale(0);
    }
    50% {
        transform: scale(1.10);
    }
    100% {
        transform: scale(1);
    }
}
</style>
