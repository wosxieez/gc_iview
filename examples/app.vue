<template>
  <div>
    <AutoTable v-bind="autoTableConfig"></AutoTable>
  </div>
</template>

<script>
export default {
  data() {
    return {
      autoTableConfig: {
        columns: [
          { title: "username", key: "username" },
          { title: "id", key: "id" }
        ],
        url: "/api/user/list",
        path: "datas"
      }
    };
  }
};
</script>

<style>
</style>
