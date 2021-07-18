<template>
  <div id="ExampleApp">
    <Card 
    title="Titulo configurable" 
    body="Lorem ipsum dolor sit amet consectetur adipiscing, eli aptent commodo tempus gravida, eleifend mollis condimentum neque sollicitudin. Elementum magnis lacinia diam eget facilisi consequat ullamcorper, litora aenean dui laoreet posuere praesent, est sed conubia scelerisque quisque semper."/>
  </div>
</template>

<script>
import Card from './components/Card.vue'

export default {
  name: 'ExampleApp',
  components: {
    Card
  }
}
</script>

<style>
#ExampleApp {
  display: flex;
  justify-content: center;
  margin-top: 60px;
}
</style>
