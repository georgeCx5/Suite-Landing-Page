<script>
import IconFacebook from '@/assets/content/icon-facebook.svg?component'
import IconTwitter from '@/assets/content/icon-twitter.svg?component'
import IconInstagram from '@/assets/content/icon-instagram.svg?component'

export default {
   props: {
      btnName: String,
   },
   components: {
      IconFacebook,
      IconTwitter,
      IconInstagram,
   }
}
</script>
<template>
   <button>
      <component :is="`Icon${btnName}`" />
   </button>
</template>