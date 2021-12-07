<template>
  <v-dialog v-model="show" width="500">
    <v-card>
      <v-card-title class="error">
        Something went wrong, please try again!
      </v-card-title>
      <v-card-text class="title pa-4">
        Your location was not found.
      </v-card-text>
      <v-card-actions>
        <v-btn @click="$emit('toggle-dialog', false)">close</v-btn>
      </v-card-actions>
    </v-card>
  </v-dialog>
</template>

<script>
export default {
  props: {
    show: Boolean
  }
};
</script>
