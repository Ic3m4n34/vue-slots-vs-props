<template>
  <div id='app'>
    <CustomButtonWithProps
      :button-text="'I\'m a button'"
    />
    <CustomButtonWithSlots />
  </div>
</template>

<script>
import CustomButtonWithProps from './components/custom-button-with-props';
import CustomButtonWithSlots from './components/custom-button-with-slots';

export default {
  name: 'App',
  components: {
    CustomButtonWithProps,
    CustomButtonWithSlots,
  },
};
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
