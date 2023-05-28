<template>
<h2>Laptops - 2023</h2>
   <div>
      <table class="table table-hover">
         <thead>
         <tr>
               <th scope="col">ID</th>
               <th scope="col">Name</th>
               <th scope="col">Price</th>
               <th scope="col">Order</th>
         </tr>
         </thead>
         <tbody v-for="product in products" :key="product.id">
            <tr>
                  <td scope="ro2">{{  product.id }}</td>
                  <td>{{ product.name }}</td>
                  <td>{{ product.price }}</td>
                  <td><button>Order</button></td>
            </tr>
         </tbody>
      </table>
   </div>
  </template>
  
  <script>
   import { products } from '@/data';
   export default {
      name: 'productsPage',
      data() {
         return { products };
      }
   }
  </script>
  
  <style scoped>
 
  </style>