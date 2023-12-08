<template>
  <div class="d-flex">
    <GoogleMap api-key="AIzaSyB1GhrKvPtal9CuIvyQYEC7hCeV9Vvq56E" style="margin: 10% 10% 10% 0; width: 580px; height: 500px"
               :center="center" :zoom="4">
      <Marker :options="{ position: center }"/>
    </GoogleMap>
    <div style="margin-top: 80px ">
      <h1 class="mt-5">Зв'язатися з нами</h1>
      <a href="#" style="font-size: 20px">Зв'яжіться з нашими менеджерами</a>
      <p class="mt-3">Наші контакти:</p>
      <div class="d-flex justify-content-between">
        <p>Kievstar:</p><a href="#" class="ml-1" style="white-space: nowrap">+380 99 893 94 98</a>
        <p style="margin-left: 13px">Life:</p><a href="#" class="ml-1" style="white-space: nowrap">+380 55 555 55 00</a>
      </div>
      <p>Наша адреса:</p>
      <p><a href="#" style="font-size: 23px">ВІТІ</a></p>
    </div>
  </div>
</template>

<script>
import {defineComponent} from "vue";
import {GoogleMap, Marker} from "vue3-google-map";
export default defineComponent({
  components: {GoogleMap, Marker},
  setup() {
    const center = {lat: -79.955729, lng: 15.808345};

    return {center};
  },
});
</script>

<style scoped>

</style>