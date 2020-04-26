<template>
  <v-app>
    <v-container fill-height fluid>
      <v-layout wrap>
        <v-flex xs12 sm9 md9 lg8 xl8>
          <input
            ref="input"
            style="display: none"
            type="file"
            accept="image/jpeg, image/jpg, image/png"
          />
          <v-card min-height="50%" @click.stop="cardClick">
            <v-card-text>
              Upload your image
            </v-card-text>
          </v-card>
        </v-flex>
      </v-layout>
    </v-container>
  </v-app>
</template>

<script>
export default {
  methods: {
    // selectfileボタン押下時
    cardClick() {
      this.$refs.input.click()
    }
  }
}
</script>
