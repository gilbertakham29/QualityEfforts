<template>
    <div class="flex flex-col items-center px-4 py-10 mx-auto border-b max-w-screen-2xl sm:px-8 border-b-gray-200">
        <h2 class="mb-10 text-3xl font-bold tracking-light text-center sm:text-4xl">
            Contact us whenever you like
        </h2>
        <form action="#" class="grid w-full grid-cols-1 gap-5 sm:grid-cols-2 sm:max-w-screen-md">
            <div class="col-span-1">
                <label for="Name" class="block mb-2 text-sm font-medium text-gray-900 dark:text-gray-300">Name</label>
                <input type="text" id="Name" value class="block w-full p-3 text-sm text-gray-900 border border-gray-300 rounded-lg shadow-sm bg-gray-50 focus:ring-primary-500 focus:border-primary-500 dark:bg-gray-700 dark:border-gray-600 dark:placeholder-gray-400 dark:text-white dark:focus:ring-primary-500 dark:focus:border-primary-500 dark:shadow-sm-light" placeholder="Let us know your name" required>
            </div>
            <div class="col-span-1">
                <label for="Email" class="block mb-2 text-sm font-medium text-gray-900 dark:text-gray-300">Email</label>
                <input type="email" id="Email" value class="block w-full p-3 text-sm text-gray-900 border border-gray-300 rounded-lg shadow-sm bg-gray-50 focus:ring-primary-500 focus:border-primary-500 dark:bg-gray-700 dark:border-gray-600 dark:placeholder-gray-400 dark:text-white dark:focus:ring-primary-500 dark:focus:border-primary-500 dark:shadow-sm-light" placeholder="name@compay.com" required>
                <span class="invisible text-sm font-medium text-red-500">
                    Email is not valid
                </span>
            </div>
            <div class="sm:col-span-2">
                <label for="message" class="block mb-2 text-sm font-medium text-gray-900 dark:text-gray-400">Message</label>
                <textarea class="block p-2.5 w-full text-sm text-gray-900 bg-gray-50 rounded-lg shadow-sm border border-gray-300 focus:ring-primary-500 focus:border-primary-500 dark:bg-gray-700 dark:border-gray-600 dark:placeholder-gray-400 dark:text-white dark:focus:ring-primary-500 dark:focus:border-primary-500" id="message" rows="6" placeholder="Please leave a message...">

                </textarea>
            </div>
            <div class="flex justify-center w-full sm:col-span-2">
                <button type="submit" class="flex items-center px-5 py-3 text-sm font-medium text-center text-white rounded-lg bg-[#299646] sm:w-fit hover:bg-green-500 focus:ring-4 focus:outline-none">
                    Send Message
                </button>
            </div>
        </form>
    </div>
</template>

<script setup>

</script>

<style  scoped>

</style>