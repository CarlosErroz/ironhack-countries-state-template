<template>
  <Navbar />
  <div class="container">
    <div class="row">
      <div class="col-5" style="max-height: 90vh; overflow: scroll">
        <CountriesList />
      </div>
      <div class="col-7">
        <CountryDetails />
      </div>
    </div>
  </div>
</template>

<script setup>
import Navbar from "./components/Navbar.vue";
import CountriesList from "./pages/CountriesList.vue";
import CountryDetails from "./pages/CountryDetails.vue";

import {useCountryStore} from './stores/country.js'
const main = useCountryStore()

/* export default {
  components: {
    Navbar,
    CountriesList,
    CountryDetails,
  },
};
*/

</script>

<style></style>
