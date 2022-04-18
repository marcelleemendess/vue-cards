<template>
  <div class="product">
    <div :class="'product-inner' + product.color">
      <div class="product-text-wrap">
        <h2 class="bg-text">{{ product.bgtext }}</h2>
      </div>
      <div class="product-image-wrap">
        <img :src="product.src" :alt="product.title" class="image" />
      </div>
      <div class="product-detail">
        <h2>{{ product.title }}</h2>
        <p>
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Beatae
          commodi inventore eos laboriosam blanditiis autem consequatur deleniti
          labore libero doloremque?
        </p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "ProductComponent",
  props: ["product"],
};
</script>
