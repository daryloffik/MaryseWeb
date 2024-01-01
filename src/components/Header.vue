<!-- eslint-disable vue/multi-word-component-names -->

<script setup>
import { ref } from 'vue'

defineProps({
list: {
type: Array,
default: () => []
},
logo: {
type: String,
default: 'none'
},
links0: {
    type: String,
    default: '#'
},
links1: {
    type: String,
    default: '#'
},
links2: {
    type: String,
    default: '#'
}
});


const show = ref(false)
</script>
<template>
<header class="flex flex-wrap flex-row justify-between mx-auto 
bg-[#ebfffd] p-4 ">
<p class="Name text-2xl p-2">
{{ logo }}
</p>
<div >
  <nav  class="lg:flex flex-row justify-center items-center hidden lg:opacity-100">
     <a
            role="menuitem"
            href=""
            class="group flex items-center justify-between rounded-lg border border-transparent px-2.5  text-lg font-medium text-gray-700 hover:bg-blue-50 hover:text-blue-800 active:border-blue-100 dark:text-gray-200 dark:hover:bg-gray-700/75 dark:hover:text-white dark:active:border-gray-600"
          >
         
            <span class="grow">Acceuil</span>
          </a>
          <a
            role="menuitem"
            href="#apropos"
            class="group flex items-center justify-between space-x-2 rounded-lg border border-transparent px-2.5 text-lg font-medium text-gray-700 hover:bg-blue-50 hover:text-blue-800 active:border-blue-100 dark:text-gray-200 dark:hover:bg-gray-700/75 dark:hover:text-white dark:active:border-gray-600"
          >
           
            <span class="grow">A propos</span>
          </a>
          <a
            role="menuitem"
            href="#work"
            class="group flex items-center justify-between space-x-2 rounded-lg border border-transparent px-2.5 py-2 text-lg font-medium text-gray-700 hover:bg-blue-50 hover:text-blue-800 active:border-blue-100 dark:text-gray-200 dark:hover:bg-gray-700/75 dark:hover:text-white dark:active:border-gray-600"
          >
         
            <span class="grow">Nos travaux</span>
          </a>
   
</nav>

</div>

<!-- Dropdowns: Simple -->
<div class="flex justify-end lg:opacity-0">
  <!-- Dropdown Container -->
  <div class="relative inline-block">
    <!-- Dropdown Toggle Button -->
    <button
      type="button"
      class="inline-flex items-center justify-center space-x-2 rounded-lg border border-gray-400  px-3 py-2 text-sm font-semibold leading-5 text-black hover:border-blue-200 hover:bg-blue-200 hover:text-white focus:ring focus:ring-blue-400 focus:ring-opacity-50 active:border-blue-700 active:bg-blue-200 dark:focus:ring-blue-400 dark:focus:ring-opacity-90"
      id="tk-dropdown"
      aria-haspopup="true"
      aria-expanded="true"
      @click="show = !show"
    >
      <span><svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-6 h-6">
  <path stroke-linecap="round" stroke-linejoin="round" d="M3.75 6.75h16.5M3.75 12h16.5m-16.5 5.25h16.5" />
</svg>
</span>
    
    </button>
    <!-- END Dropdown Toggle Button -->

    <!-- Dropdown -->
    <!-- 
      Visibility
        Closed        'hidden'
        Opened        '' (no class)

      Show/Hide with transitions
        enter         'transition ease-out duration-100'
        enter-start   'opacity-0 scale-90'
        enter-end     'opacity-100 scale-100'
        leave         'transition ease-in duration-75'
        leave-start   'opacity-100 scale-100'
        leave-end     'opacity-0 scale-90'
    -->
    <div
      role="menu"
      aria-labelledby="tk-dropdown"
      class="absolute right-0 z-10 mt-2 w-48 origin-top-right rounded-lg shadow-xl dark:shadow-gray-900 "
      v-if="show"
    >
      <div
        class="divide-y divide-gray-100 rounded-lg bg-white ring-1 ring-black ring-opacity-5 dark:divide-gray-700 dark:bg-gray-800 dark:ring-gray-700 hover:text-blue-500"
      >
        <div class="">
          <a
            role="menuitem"
            href=""
            class="group flex items-center justify-between space-x-2 rounded-lg border border-transparent px-2.5 py-2 text-sm font-medium text-gray-700 hover:bg-blue-50 hover:text-blue-800 active:border-blue-100 dark:text-gray-200 dark:hover:bg-gray-700/75 dark:hover:text-white dark:active:border-gray-600"
          >
         
            <span class="grow">Acceuil</span>
          </a>
        </div>
        <div >
          <a
            role="menuitem"
            href="#apropos"
            class="group flex items-center justify-between space-x-2 rounded-lg border border-transparent px-2.5 py-2 text-sm font-medium text-gray-700 hover:bg-blue-50 hover:text-blue-800 active:border-blue-100 dark:text-gray-200 dark:hover:bg-gray-700/75 dark:hover:text-white dark:active:border-gray-600"
          >
           
            <span class="grow">A propos</span>
          </a>
          <a
            role="menuitem"
            href="#work"
            class="group flex items-center justify-between space-x-2 rounded-lg border border-transparent px-2.5 py-2 text-sm font-medium text-gray-700 hover:bg-blue-50 hover:text-blue-800 active:border-blue-100 dark:text-gray-200 dark:hover:bg-gray-700/75 dark:hover:text-white dark:active:border-gray-600"
          >
         
            <span class="grow">Nos travaux</span>
          </a>
          <a
            role="menuitem"
            href="https://web.facebook.com/mayola.maryse"
            class="group flex items-center justify-between space-x-2 rounded-lg border border-transparent px-2.5 py-2 text-sm font-medium text-gray-700 hover:bg-blue-50 hover:text-blue-800 active:border-blue-100 dark:text-gray-200 dark:hover:bg-gray-700/75 dark:hover:text-white dark:active:border-gray-600"
          >
          <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-facebook" viewBox="0 0 16 16">
  <path d="M16 8.049c0-4.446-3.582-8.05-8-8.05C3.58 0-.002 3.603-.002 8.05c0 4.017 2.926 7.347 6.75 7.951v-5.625h-2.03V8.05H6.75V6.275c0-2.017 1.195-3.131 3.022-3.131.876 0 1.791.157 1.791.157v1.98h-1.009c-.993 0-1.303.621-1.303 1.258v1.51h2.218l-.354 2.326H9.25V16c3.824-.604 6.75-3.934 6.75-7.951"/>
</svg>
            <span class="grow">Facebook</span>
          </a>
          <a
            role="menuitem"
            href="https://www.linkedin.com/in/mayola-maryse-aniambossou-1690751bb?lipi=urn%3Ali%3Apage%3Ad_flagship3_profile_view_base_contact_details%3BvDrcQFY9RRCX93GpPDHwzw%3D%3D"
            class="group flex items-center justify-between space-x-2 rounded-lg border border-transparent px-2.5 py-2 text-sm font-medium text-gray-700 hover:bg-blue-50 hover:text-blue-800 active:border-blue-100 dark:text-gray-200 dark:hover:bg-gray-700/75 dark:hover:text-white dark:active:border-gray-600"
          >
          <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-linkedin" viewBox="0 0 16 16">
  <path d="M0 1.146C0 .513.526 0 1.175 0h13.65C15.474 0 16 .513 16 1.146v13.708c0 .633-.526 1.146-1.175 1.146H1.175C.526 16 0 15.487 0 14.854V1.146zm4.943 12.248V6.169H2.542v7.225h2.401m-1.2-8.212c.837 0 1.358-.554 1.358-1.248-.015-.709-.52-1.248-1.342-1.248-.822 0-1.359.54-1.359 1.248 0 .694.521 1.248 1.327 1.248h.016zm4.908 8.212V9.359c0-.216.016-.432.08-.586.173-.431.568-.878 1.232-.878.869 0 1.216.662 1.216 1.634v3.865h2.401V9.25c0-2.22-1.184-3.252-2.764-3.252-1.274 0-1.845.7-2.165 1.193v.025h-.016a5.54 5.54 0 0 1 .016-.025V6.169h-2.4c.03.678 0 7.225 0 7.225h2.4"/>
</svg>
            <span class="grow">Linkedin</span>
          </a>
          <a
            role="menuitem"
            href="https://mobile.twitter.com/MaryseMayola"
            class="group flex items-center justify-between space-x-2 rounded-lg border border-transparent px-2.5 py-2 text-sm font-medium text-gray-700 hover:bg-blue-50 hover:text-blue-800 active:border-blue-100 dark:text-gray-200 dark:hover:bg-gray-700/75 dark:hover:text-white dark:active:border-gray-600"
          >
          <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-twitter" viewBox="0 0 16 16">
  <path d="M5.026 15c6.038 0 9.341-5.003 9.341-9.334 0-.14 0-.282-.006-.422A6.685 6.685 0 0 0 16 3.542a6.658 6.658 0 0 1-1.889.518 3.301 3.301 0 0 0 1.447-1.817 6.533 6.533 0 0 1-2.087.793A3.286 3.286 0 0 0 7.875 6.03a9.325 9.325 0 0 1-6.767-3.429 3.289 3.289 0 0 0 1.018 4.382A3.323 3.323 0 0 1 .64 6.575v.045a3.288 3.288 0 0 0 2.632 3.218 3.203 3.203 0 0 1-.865.115 3.23 3.23 0 0 1-.614-.057 3.283 3.283 0 0 0 3.067 2.277A6.588 6.588 0 0 1 .78 13.58a6.32 6.32 0 0 1-.78-.045A9.344 9.344 0 0 0 5.026 15"/>
</svg>
            <span class="grow">Twitter</span>
          </a>
        </div>
      
      </div>
    </div>
    <!-- END Dropdown -->
  </div>
  <!-- Dropdown Container -->
</div>
<!-- END Dropdowns: Simple -->
<nav  class="lg:flex lg:flex-row lg:justify-end lg:items-center hidden lg:opacity-100 lg:mr-10 ">
  <a
            role="menuitem"
            href="https://web.facebook.com/mayola.maryse"
            class="group flex items-center justify-between space-x-2 rounded-lg border border-transparent px-2.5 py-2 text-sm font-medium text-gray-700 hover:bg-blue-50 hover:text-blue-800 active:border-blue-100 dark:text-gray-200 dark:hover:bg-gray-700/75 dark:hover:text-white dark:active:border-gray-600"
          >
          <svg xmlns="http://www.w3.org/2000/svg" width="26" height="26" fill="currentColor" class="bi bi-facebook" viewBox="0 0 16 16">
  <path d="M16 8.049c0-4.446-3.582-8.05-8-8.05C3.58 0-.002 3.603-.002 8.05c0 4.017 2.926 7.347 6.75 7.951v-5.625h-2.03V8.05H6.75V6.275c0-2.017 1.195-3.131 3.022-3.131.876 0 1.791.157 1.791.157v1.98h-1.009c-.993 0-1.303.621-1.303 1.258v1.51h2.218l-.354 2.326H9.25V16c3.824-.604 6.75-3.934 6.75-7.951"/>
</svg>
            
          </a>
          <a
            role="menuitem"
            href="https://www.linkedin.com/in/mayola-maryse-aniambossou-1690751bb?lipi=urn%3Ali%3Apage%3Ad_flagship3_profile_view_base_contact_details%3BvDrcQFY9RRCX93GpPDHwzw%3D%3D"
            class="group flex items-center justify-between space-x-2 rounded-lg border border-transparent px-2.5 py-2 text-sm font-medium text-gray-700 hover:bg-blue-50 hover:text-blue-800 active:border-blue-100 dark:text-gray-200 dark:hover:bg-gray-700/75 dark:hover:text-white dark:active:border-gray-600"
          >
          <svg xmlns="http://www.w3.org/2000/svg" width="26" height="26" fill="currentColor" class="bi bi-linkedin" viewBox="0 0 16 16">
  <path d="M0 1.146C0 .513.526 0 1.175 0h13.65C15.474 0 16 .513 16 1.146v13.708c0 .633-.526 1.146-1.175 1.146H1.175C.526 16 0 15.487 0 14.854V1.146zm4.943 12.248V6.169H2.542v7.225h2.401m-1.2-8.212c.837 0 1.358-.554 1.358-1.248-.015-.709-.52-1.248-1.342-1.248-.822 0-1.359.54-1.359 1.248 0 .694.521 1.248 1.327 1.248h.016zm4.908 8.212V9.359c0-.216.016-.432.08-.586.173-.431.568-.878 1.232-.878.869 0 1.216.662 1.216 1.634v3.865h2.401V9.25c0-2.22-1.184-3.252-2.764-3.252-1.274 0-1.845.7-2.165 1.193v.025h-.016a5.54 5.54 0 0 1 .016-.025V6.169h-2.4c.03.678 0 7.225 0 7.225h2.4"/>
</svg>

          </a>
          <a
            role="menuitem"
            href="https://mobile.twitter.com/MaryseMayola"
            class="group flex items-center justify-between space-x-2 rounded-lg border border-transparent px-2.5 py-2 text-lg font-medium text-gray-700 hover:bg-blue-50 hover:text-blue-800 active:border-blue-100 dark:text-gray-200 dark:hover:bg-gray-700/75 dark:hover:text-white dark:active:border-gray-600"
          >
          <svg xmlns="http://www.w3.org/2000/svg" width="26" height="26" fill="currentColor" class="bi bi-twitter" viewBox="0 0 16 16">
  <path d="M5.026 15c6.038 0 9.341-5.003 9.341-9.334 0-.14 0-.282-.006-.422A6.685 6.685 0 0 0 16 3.542a6.658 6.658 0 0 1-1.889.518 3.301 3.301 0 0 0 1.447-1.817 6.533 6.533 0 0 1-2.087.793A3.286 3.286 0 0 0 7.875 6.03a9.325 9.325 0 0 1-6.767-3.429 3.289 3.289 0 0 0 1.018 4.382A3.323 3.323 0 0 1 .64 6.575v.045a3.288 3.288 0 0 0 2.632 3.218 3.203 3.203 0 0 1-.865.115 3.23 3.23 0 0 1-.614-.057 3.283 3.283 0 0 0 3.067 2.277A6.588 6.588 0 0 1 .78 13.58a6.32 6.32 0 0 1-.78-.045A9.344 9.344 0 0 0 5.026 15"/>
</svg><span class="grow"></span>
          </a>
   
</nav>
 
</header> 
</template>

<style>
  @import url('https://fonts.googleapis.com/css2?family=Dancing+Script&family=Inconsolata:wght@800&display=swap');

  .Name{
    font-family: 'Inconsolata',monospace;
  }

  
</style>
