<template>
  <main id="app">
    <section class="products">
      <ProductComponent
        v-for="product in products"
        :key="product.id"
        :product="product"
      />
    </section>
  </main>
</template>

<script>
import ProductComponent from "./components/ProductComponent";

export default {
  name: "App",
  components: {
    ProductComponent,
  },
  data() {
    return {
      products: [
        {
          id: 1,
          title: "Nike Air Max",
          color: "green",
          bgtext: "NIKE",
          src: require("./assets/img/green-shoe.png"),
        },
        {
          id: 2,
          title: "Nike flex",
          color: "blue",
          bgtext: "AIR",
          src: require("./assets/img/blue-shoe.png"),
        },
        {
          id: 3,
          title: "Nike Roche Runs",
          color: "pink",
          bgtext: "MAX",
          src: require("./assets/img/pink-shoe.png"),
        },
      ],
    };
  },
};
</script>
