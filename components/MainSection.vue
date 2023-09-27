<template>
    <div class="bg-[#000837] py-1 grid grid-cols-2">
       
        <div class="grid grid-cols-1 w-11/12 md:w-10/12 border-r-2 border-r-white mx-auto text-white text-xl md:text-3xl md:gap-x-16 gap-y-10 mt-10  mb-20 md:mb-52">
            <div class="col-span-12 md:col-span-6 flex items-center">
                <h2 class=" text-center text-3xl md:text-6xl font-bold text-[#FAC300] my-8 md:my-16 pt-10">
            Our Experience
        </h2>
            </div>
            <div class="col-span-1 sm:col-span-1 md:col-span-6">
                <img src="https://save-effort.netlify.app/_nuxt/p1.083a4428.webp" alt="settings"/>
                <p class="ml-2">200+ Processes automated</p>
            </div>
            <div class="col-span-12 md:col-span-6 ">
                <img src="data:image/webp;base64,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" alt="digital"/>
                <p class="ml-2">10+ Digital Platform delivered</p>
            </div>
            <div class="col-span-12 md:col-span-6">
                <img src="https://save-effort.netlify.app/_nuxt/p1.083a4428.webp" alt="settings"/>
                <p class="ml-2">100+ platforms integrated</p>
            </div>
            <div class="col-span-12 md:col-span-6 ">
                <img src="data:image/webp;base64,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" alt="cleints"/>
                <p class="ml-2">50+ Clients</p>
            </div>
        </div>
        <div class=" bg-[#000837]">
        <button type="button" data-modal-target="authentication-modal" data-modal-toggle="authentication-modal" class="flex items-center w-auto px-8 py-3 mx-auto my-auto font-medium text-center text-white rounded-lg sm:mt-5 lg:mt-96 sm:ml-auto lg:ml-auto sm:mb-10 lg:mb-10 bg-[#FAC300] sm:w-fit hover:bg-yellow-400 focus:ring-4 focus:outline-none mt-96">
        Discover More
    </button>
    </div>
    </div>
  
   

    <div id="authentication-modal" tabindex="-1" aria-hidden="true" class="fixed left-0 right-0 z-50 w-full max-h-full p-4 overflow-x-hidden overflow-y-auto bg-gray-100 top-[12.5%] md:top-0 md:inset-0 bg-opacity-20 justify-center items-center hidden">
    <div class="relative w-full max-w-md max-h-full">
        <!-- Modal content -->
        <div class="relative bg-white rounded-lg shadow ">
            <button type="button" class="absolute top-3 right-2.5 text-gray-400 bg-transparent hover:bg-gray-200 hover:text-gray-900 rounded-lg text-sm w-8 h-8 ml-auto inline-flex justify-center items-center" data-modal-hide="authentication-modal">
                <svg class="w-3 h-3" aria-hidden="true" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 14 14">
                    <path stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="m1 1 6 6m0 0 6 6M7 7l6-6M7 7l-6 6"/>
                </svg>
                <span class="sr-only">Close modal</span>
            </button>
            <div class="px-6 py-6 lg:px-8">
                <h3 class="mb-4 text-xl font-medium text-gray-900 dark:text-white">Contact us</h3>
                <form class="space-y-6" action="#">
                    <div class="col-span-1">
                        <label for="Name" class="block mb-2 text-sm font-medium text-gray-900 dark:text-gray-300">Name</label>
                        <input type="text" id="name" class="block w-full p-3 text-sm text-gray-900 border border-gray-300 rounded-lg shadow-sm bg-gray-50 focus:ring-primary-500 focus:border-primary-500 dark:bg-gray-700 dark:border-gray-600 dark:placeholder-gray-400 dark:text-white dark:focus:ring-primary-500 dark:focus:border-primary-500 dark:shadow-sm-light" placeholder="Let us know your name" required>
                    </div>
                    <div class="col-span-1">
                        <label for="email" class="block mb-2 text-sm font-medium text-gray-900 dark:text-gray-300">Email</label>
                        <input type="email" id="email" placeholder="name@company.com" class="block w-full p-3 text-sm text-gray-900 border-2 border-gray-300 rounded-lg shadow-sm bg-gray-50 focus:ring-white focus:border-primary-500" required>
                        <span class="invisible text-sm font-medium text-red-50">Email is not valid</span>
                    </div>
                    <div class="sm:col-span-2">
                        <label for="message" class="block mb-2 text-sm font-medium text-gray-900 dark:text-gray-400">Message</label>
                        <textarea id="message" rows="6" class="block p-2.5 w-full text-sm text-gray-900 bg-gray-50 rounded-lg shadow-sm border border-gray-300 focus:ring-primary-500 focus:border-primary-500 dark:bg-gray-700 dark:border-gray-600 dark:placeholder-gray-400 dark:text-white dark:focus:ring-primary-500 dark:focus:border-primary-500" required placeholder="Please leave a message..."></textarea>
                    </div>
                    <div class="flex justify-center w-full sm:col-span-2">
                        
                    <button type="submit" class="flex items-center px-5 py-3 text-sm font-medium text-center text-white rounded-lg bg-[#FAC300] sm:w-fit hover:bg-yellow-400 focus:ring-4 focus:outline-none">
                        <span>Send Message</span>
                    </button>    
                    </div>
                    
                </form>
            </div>
        </div>
    </div>
</div>
</template>

<script setup>

</script>

<style  scoped>

</style>