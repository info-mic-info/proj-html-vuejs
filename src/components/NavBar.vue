<script>
export default {
  props: {
    itemsNav: Object,
  },
};
</script>


<template lang="">
<li class="mx-4">{{itemsNav.label}}</li>

</template>


<style lang="scss" scoped>
li:hover {
  color: orange;
}
</style>