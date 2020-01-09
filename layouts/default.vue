<template>
  <v-app>
    <TheHeader/>
    <Left />
    <nuxt/>
    <Right />
  </v-app>
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

<style>
html {
  font-family: 'M PLUS Rounded 1c', sans-serif, 'Source Sans Pro', -apple-system, BlinkMacSystemFont, 'Segoe UI',
    Montserrat, 'Helvetica Neue', Arial, sans-serif, ;
  font-size: 16px;
  word-spacing: 1px;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
  background-color:#fff;
  color : ＃808080
}

*,
*:before,
*:after {
  box-sizing: border-box;
  margin: 0;
}
.container {
  padding: 80px 50px 60px 50px;
  height: 100%;
  text-align: center;
}
.v-application--wrap{
  background-color:#fff;
}
.v-application a{
  text-decoration:none;
}
</style>