<!-- eslint-disable vue/multi-word-component-names -->
<template>
       <div class="mt-10 m-2">
    <h1 class="text-blue-500 font-extrabold text-[50px]">Nos travaux.
    </h1>
    <div class="lg:max-w-[1002px]">
        A travers  <a
            role="menuitem"
            href="https://www.youtube.com/@InstantFiscalbenin"
            class="cursor-pointer"
          > <span>  Instant fiscal</span></a> ,Mon équipe et moi avons pour objectif de  fournir des conseils précis et stratégiques pour optimiser la conformité fiscale et les opportunités commerciales.
        <div class="list flex flex-col gap-4 mt-5 m-4 items-center lg:flex lg:flex-row">
    <div>
      <video src="/public/video_2023-11-16_13-53-21.mp4" class="w-[1300px]"></video>
    </div>
    <div>
      <video src="/public/video_2023-11-16_14-53-23.mp4" ></video>
    </div>
    <div>
      <video src="/public/video_2023-11-16_15-02-59.mp4"></video>
      
    </div>
     <div class="voir">
        <a
            role="menuitem"
            href="https://www.youtube.com/@InstantFiscalbenin"
            class="group flex items-center justify-between space-x-2 rounded-lg border border-transparent px-2.5 py-2 text-sm font-medium text-gray-700  hover:text-blue-800 active:border-blue-100 dark:text-gray-200 dark:hover:bg-gray-700/75 dark:hover:text-white dark:active:border-gray-600"
          >
        <button type="button" class="  border-[1px] border-blue-500 w-44 h-10 rounded-xl  bg-transparent z-10 ">
            Voir plus
        </button>
      
    </a>
    <div class="w-44 h-10 bg-blue-400 mt-5 ml-5 mb-3 rounded-xl z-0 ">

</div>
     </div>
    </div>
</div>
   </div>
</template>


<style scoped>
.voir{
    display:grid;
    place-content: center;
  }
  .voir > * {
    grid-area: 1/1;
  }
</style>