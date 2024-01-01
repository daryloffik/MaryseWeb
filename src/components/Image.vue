<!-- eslint-disable vue/multi-word-component-names -->
<template >
    <div class="flex max-w-[300px]  flex-col justify-center items-stretch pl-3.5 single  ">
        <div class="aspect-[1.03] w-[300px] border-2 mr-10    rounded-full">
            <img
        loading="lazy"
        srcSet="public/maryse.jpeg"
        class="aspect-[1.03] object-contain rounded-full object-center w-full overflow-hidden max-md:max-w-full"
      />
</div>
    
      <div class="aspect-[1.03] w-[300px] border-2 mr-10 rotate-45  border-[#098FBA] rounded-full">

      </div>
      <img src="/Group 6.png" alt="" class="w-15 h-5 lg:w-20 mt-56">
      <img src="/Group 10.png" alt="" class="w-15 h-10 ml-72 lg:w-16 lg:h-16">
    </div>
  </template>

  <style scoped>
  .single{
    display:grid;
    place-content: center;
  }
  .single > * {
    grid-area: 1/1;
  }
  </style>