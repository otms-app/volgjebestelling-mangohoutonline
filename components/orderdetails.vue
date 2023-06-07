<template>
  <div class="container col-md-12">
    <div class="form-body">
      <h2 class="halloklant">Hallo {{}},</h2>
      <p class="dankjewel">
        Bedankt voor je bestelling bij Mangohoutonline. We doen ons uiterste
        best om je bestelling zo snel mogelijk bij je af te leveren. Hierbij
        proberen we je zo goed mogelijk op de hoogte te houden van de status. Je
        bestelling wordt geleverd op het moment dat alle producten op voorraad
        zijn.
      </p>
    </div>
    <table class="table">
      <thead>
        <tr>
          <th></th>
          <th>Product</th>
          <th>SKU</th>
          <th>Status</th>
        </tr>
      </thead>
      <tbody>
        <tr v-for="item in items" :key="item.sku">
          <td><i class="fa fa-truck"></i></td>
          <td>{{ item.sku }}</td>
          <td>{{ item.name }}</td>
          <td>{{ item.stock_status }}</td>
        </tr>
      </tbody>
    </table>
  </div>
</template>

<script>
import { inject } from 'vue';

export default {};
</script>

<style>
.halloklant {
  margin-bottom: 20px;
}

.dankjewel {
  color: #777;
  margin-bottom: 20px;
}

.td {
  font-size: 14px;
  color: #777;
}
</style>
