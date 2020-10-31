<template>
  <li class="d-flex align-items-center list-group-item">
    <button class="btn flex-grow-1 border-0 text-left">
      {{ data }}
    </button>
    <form class="flex-grow-1">
      <input type="text" class="form-control" />
    </form>
    <button class="btn btn-secondary">Edit</button>
    <button @click="$emit('on-delete')" class="btn btn-secondary">
      Delete
    </button>
  </li>
</template>



<script>
export default {
  props: {
    data: String,
    complete: Boolean,
  },
  data() {
    return {
      editing: false,
      new_goal: "",
    };
  },
};
</script>


<style >
.completed {
  text-decoration: line-through;
}
</style>