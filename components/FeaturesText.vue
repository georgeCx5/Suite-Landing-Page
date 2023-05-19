<script>
export default {
   props: {
      text1: String,
      text2: String,
   }
}
</script>
<template>
   <div class=" flex flex-col items-center gap-[1px]">
      <h3 class=" text-neo-dark-blue text-[48px] leading-[56px] font-bold">{{ text1 }}</h3>
      <h5 class=" text-neo-light-blue text-[16px] leading-[28px] tracking-[2.5px] uppercase">{{ text2 }}</h5>
   </div>
</template>