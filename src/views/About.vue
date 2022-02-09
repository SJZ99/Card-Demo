<template>
  <div class="about">
    <v-card width=300 id="card">
      <v-img src="../assets/keyboard.jpg"></v-img>

      <v-card-title>
        Title
      </v-card-title>


      <v-card-actions>

        <v-spacer></v-spacer>

        <v-btn icon @click="isActive = !isActive">
          <v-icon :class="{ active : isActive }">mdi-cards-heart</v-icon>
        </v-btn>

        <v-btn icon>
          <v-icon>mdi-bookmark</v-icon>
        </v-btn>

        <v-btn icon>
          <v-icon>mdi-share-variant</v-icon>
        </v-btn>
      </v-card-actions>
    </v-card>
  </div>
</template>

<script>
export default {
  data: () => ({
    isActive: false,
  })
}
</script>

<style>
#card {
  margin: 0 auto;
}
.active{ 
  color: rgb(255, 0, 0) !important;
}
</style>
