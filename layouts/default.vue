<template>
  <div>
    <TheHeader/>
    <Left />
 
      <nuxt/>
    <Right />
 
  </div>
</template>

<script>
  import TheHeader from '~/components/common/TheHeader';
  import TheFooter from '~/components/common/TheFooter';
  import Left from '~/components/common/Left';
  import Right from '~/components/common/Right';

  export default {
    components: {
      TheHeader,
      TheFooter,
      Left,
      Right
    }
  }
</script>