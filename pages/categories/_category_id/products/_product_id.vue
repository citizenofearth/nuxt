<template>
  <section class="container">
    <h2 class="title">_product_id.vue</h2>
    <span>Category ID: {{ $route.params.category_id }}</span>
    <span>Product ID: {{ $route.params.product_id }}</span>
  </section>
</template>

<script>
export default {
  validate({ params }) {
    // Must be a number
    return /^\d+$/.test(params.product_id)
  }
}
</script>
