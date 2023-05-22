<script>
// components
import FeaturesText from './components/FeaturesText.vue'
import BtnIcon from './components/BtnIcon.vue'
// hybrids
import Logo from '@/assets/content/logo.svg?component'
// SVG's
import curvedBlack from '@/assets/content/pattern-curved-line-1.svg?url'
import curvedCream from '@/assets/content/pattern-curved-line-2.svg?url'
import blurEffect from '@/assets/content/pattern-blur.svg?url'
// images
import phoneShortImg from '@/assets/content/image-hero-landscape.png'
import phoneLongImg from '@/assets/content/image-hero-portrait.png'
import jeremySmallImg from '@/assets/content/image-jeremy-small.png'


export default {
  data() {
    return {
      curvedBlack,
      curvedCream,
      blurEffect,
      phoneShortImg,
      phoneLongImg,
      jeremySmallImg,
      btnText: 'Request Beta Access',
    }
  },
  components: {
    FeaturesText,
    BtnIcon,
    // SGV's
    Logo,
  }
}
</script>
<template>
  <body class=" flex flex-col bg-neo-cream-white font-epilogue">
    <header
      class=" flex flex-col gap-[56px] tb:gap-[80px] mb-[56px] tb:mb-[92px] dsk:mb-[144px] px-4 tb:px-[40px] dsk:px-[166px] pt-6 tb:pt-10 dsk:pt-[50px]">
      <div class=" flex justify-between items-center">
        <Logo />
        <button
          class=" w-[182px] tb:w-[219px] h-[48px] tb:h-[56px] hover:bg-neo-dark-blue hover:text-neo-cream-white text-[14px] tb:text-[16px] font-bold leading-[24px] tb:leading-[32px] tracking-[-0.14px] tb:tracking-[-0.16px] border border-neo-dark-blue rounded-md">
          {{ btnText }}
        </button>
      </div>
      <!-- title -->
      <div class=" dsk:flex dsk:gap-24 dsk:justify-between dsk:h-[600px]">
        <div class=" relative flex flex-col gap-[32px] tb:gap-[40px] dsk:w-[824px] pt-[27px] tb:pt-[88px]">
          <img
            class=" absolute top-[0px] tb:top-[42px] left-[154px] tb:left-[222px] dsk:left-[292px] w-[151px] tb:w-[231px] dsk:w-[287px] h-[19px] tb:h-[29px] dsk:h-[36px] z-50"
            :src="curvedBlack" alt="curvedBlack">
          <h1
            class=" tb:w-[530px] dsk:w-[640px] text-[38px] tb:text-[56px] dsk:text-[72px] leading-[44px] tb:leading-[64px] dsk:leading-[78px] tracking-[-0.53px] tb:tracking-[-0.78px] dsk:tracking-[-1px] z-50">
            A <span class=" font-bold">super solution</span> for
            your
            <span class=" font-bold">business.</span>
          </h1>
          <p
            class=" tb:w-[350px] text-neo-light-blue text-[16px] dsk:text-[18px] leading-[28px] dsk:leading-[32px] tracking-[-0.09px]">
            Our marketing and sales automations help you scale your outreach to
            get more leads for your company.
          </p>
          <button
            class=" w-[256px] h-[61px] bg-neo-dark-blue hover:bg-gradient-to-br hover:from-neo-purple hover:via-neo-pink hover:to-neo-yellow text-neo-cream text-[18px] font-bold leading-[32px] tracking-[-0.18px] rounded-md">
            {{ btnText }}
          </button>
          <img class=" absolute top-0 right-0 hidden tb:block w-[281px] dsk:w-[350px]" :src="phoneLongImg"
            alt="phoneLongImg">
          <img class=" tb:hidden w-[343px] pt-6" :src="phoneShortImg" alt="phoneShortImg">
        </div>
        <!-- phoneImg -->
        <div
          class=" flex flex-col tb:flex-row dsk:flex-col tb:justify-center items-center gap-8 tb:gap-32 dsk:gap-[63px] pt-[56px] tb:pt-[123px] dsk:pt-0 dsk:-mt-3 dsk:pr-[75px]">
          <FeaturesText text1="2K+" text2="Companies" />
          <FeaturesText text1="8" text2="Languages" />
          <FeaturesText text1="1.2M" text2="Leads" />
        </div>
      </div>
    </header>
    <main class=" relative flex flex-col items-center h-[929px] tb:h-[865px] dsk:h-[600px]">
      <img class=" absolute top-2 dsk:top-auto dsk:bottom-0 dsk:left-[20%] dsk:w-[360px] z-50" :src="jeremySmallImg"
        alt="jeremySmallImg">
      <img class=" absolute top-24 tb:top-8 dsk:top-auto dsk:bottom-0 dsk:left-[15%] w-[500px]  z-40" :src="blurEffect"
        alt="blurEffect">
      <!-- bg-light-blue -->
      <div
        class=" absolute bottom-0 flex dsk:justify-end dsk:w-[1109px] h-[748px] tb:h-[684px] dsk:h-[545px] bg-neo-dark-blue tb:mx-10 dsk:mx-[167px] rounded-[15px] z-30">
        <div
          class=" flex flex-col dsk:flex-row items-center gap-[37px] dsk:gap-[53px] pt-[261px] dsk:pt-0 dsk:pr-[125px]">
          <img class=" w-[49px] dsk:w-[64px] h-[40px] dsk:h-[52px]" :src="curvedCream" alt="curvedCream">
          <div
            class=" flex flex-col justify-between dsk:w-[350px] h-[346px] tb:h-[282px] dsk:h-[369px] text-center dsk:text-left">
            <h2 class=" text-neo-cream-white text-[40px] dsk:text-[48px] leading-[48px] tracking-[-0.42px]">It just <span
                class=" font-bold">works.</span></h2>
            <p
              class=" px-4 tb:px-[58px] dsk:px-[0px] text-neo-cream text-[18px] dsk:text-[20px] leading-[32px] dsk:leading-[35px] tracking-[0.09px] dsk:tracking-[0.1px]">
              “I really like how it is an all-in-one solution that handle many of
              the tasks that you would normally need separate tools to do the same
              job. This thing is a miracle worker.”
            </p>
            <div class=" uppercase">
              <h4 class=" text-neo-cream-white text-[18px] font-bold leading-8 tracking-[-0.18px]">Jeremy Robinson</h4>
              <h5 class=" text-neo-cream text-[16px] leading-[26px] tracking-[2.5px]">CMO, Fylo</h5>
            </div>
          </div>
        </div>
      </div>
    </main>
    <footer class=" relative flex justify-center h-[230px] tb:h-[104px] mt-[56px] tb:mt-[72px] dsk:mt-[95px]">
      <div class=" absolute bottom-0 w-full h-[420px] tb:h-[640px] dsk:h-[464px] bg-neo-cream z-10"></div>
      <div
        class=" flex flex-col tb:flex-row justify-between items-center w-[125px] tb:w-full h-[150px] tb:h-[32px] tb:px-10 dsk:px-[167px] z-20">
        <Logo />
        <h3 class=" text-neo-light-blue text-[15px]">Copyright - Suite</h3>
        <div class=" flex justify-between w-full tb:w-[116px]">
          <BtnIcon btnName="Facebook" />
          <BtnIcon btnName="Twitter" />
          <BtnIcon btnName="Instagram" />
        </div>
      </div>
    </footer>
  </body>
</template>