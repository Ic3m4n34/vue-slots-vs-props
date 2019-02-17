<template>
  <div id="app">
    <CustomButtonWithProps
      :button-text="'I\'m a button'"
      :show-icon-before="true"
      :show-icon-after="true"
    />
    <CustomButtonWithSlots>
      <template v-slot:icon-before>
        <i class="fas fa-user"></i>
      </template>
      <template v-slot:button-text>
        Completely different text
      </template>
      <template v-slot:icon-after>
        <i class="fas fa-cog"></i>
      </template>
    </CustomButtonWithSlots>
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
@import 'https://use.fontawesome.com/releases/v5.7.2/css/all.css';

#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

#app > div {
  margin-bottom: 36px;
}
</style>
