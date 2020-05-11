<template>
  <div class="help">
    <h1>Help page</h1>
    <b-button size="sm" @click="toggle">
        {{ show ? 'Hide' : 'Show' }} Alert
    </b-button>
    <b-alert
        v-model="show"
        class="mt-3"
        dismissible
        @dismissed="dismissed">Hello {{ name }}!
    </b-alert>
  </div>
</template>

<script>
export default {
  name: "Help"
};
</script>

<style></style>
