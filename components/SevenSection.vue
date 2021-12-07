<template>
  <div class="py-9">
    <v-container>
      <v-row class="intro">
        <v-col cols="12">
          <h2>Contact</h2>
          <p>
            Excepteur sint occaecat cupidatat non proident, sunt in culpa qui
            officia deserunt mollit anim id est laborum. Sed ut perspiciatis
            unde omnis iste natur
          </p>
        </v-col>
      </v-row>
      <v-row>
        <v-col md="8" offset-md="2">
          <v-form ref="form" v-model="valid" lazy-validation>
            <v-text-field
              v-model="name"
              :rules="nameRules"
              label="Name *"
              outlined
              dense
              required
            ></v-text-field>

            <v-text-field
              v-model="email"
              :rules="emailRules"
              label="E-mail *"
              outlined
              dense
              required
            ></v-text-field>
            <v-textarea
              outlined
              dense
              :rules="nameRules"
              name="input-7-4"
              label="Message *"
              required
            ></v-textarea>
            <div class="d-flex justify-center">
              <v-btn
                :disabled="!valid"
                class="mr-4 btn"
                large
                @click="validate"
              >
                Send
              </v-btn>
            </div>
          </v-form>
        </v-col>
      </v-row>
    </v-container>
  </div>
</template>
<script>
export default {
  data: () => ({
    valid: true,
    name: '',
    nameRules: [
      (v) => !!v || 'Field is required',
      (v) => (v && v.length <= 10) || 'Name must be less than 10 characters',
    ],
    email: '',
    emailRules: [
      (v) => !!v || 'E-mail is required',
      (v) => /.+@.+\..+/.test(v) || 'E-mail must be valid',
    ],
    select: null,
    items: ['Item 1', 'Item 2', 'Item 3', 'Item 4'],
    checkbox: false,
  }),

  methods: {
    validate() {
      this.$refs.form.validate()
    },
    reset() {
      this.$refs.form.reset()
    },
    resetValidation() {
      this.$refs.form.resetValidation()
    },
  },
}
</script>
