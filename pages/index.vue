<template>
  <div>
  <Header />
  <div class="container">
    <h1 class="filter-header">Filters</h1>
    <Shapes />
    <Colors />
    <ShapesShapeItem />
  </div>
  </div>
</template>

<script>
import Shapes from "../components/Shapes/Shapes.vue";
export default {
    name: "IndexPage",
    components: { Shapes }
}
</script>
