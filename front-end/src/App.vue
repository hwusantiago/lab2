<template>
  <menuBar />
  <router-view></router-view>
  <div class="center-bar">
    <footer>
        <p style="text-align:center">Copyright &copy; 2023 - F28IR</p>
    </footer>
  </div>
</template>

<script>
import menuBar from '@/components/menuBar.vue';
export default {
  name: 'App',
  components: { menuBar }
}
</script>

<style>

</style>
