<template>
  <SearchFormSteps />
  <OrderDetails />
</template>

<script>
import 'bootstrap/dist/css/bootstrap.css';

import { provide, ref } from 'vue';
import SearchFormSteps from './components/searchformsteps.vue';
import OrderDetails from './components/orderdetails.vue';

export default {
  components: {
    SearchFormSteps,
    OrderDetails,
  },
  setup() {
    const fetchedData = ref(null);

    // Assuming you have a method or logic to fetch the data
    const fetchData = async () => {
      // Fetch the data and assign it to fetchedData
    };

    provide('fetchedData', fetchedData);

    return {
      fetchData,
    };
  },
};
</script>
