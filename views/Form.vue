<template>
  <div>
    <b-form class="mt-2">
      <b-row>
        <b-col class="col-6 offset-sm-3">
          <b-form-group
            label="Tarefa:"
            label-for="subject"
          >
            <b-form-input
              id="subject"
              v-model="form.subject"
              type="text"
              placeholder="Tarefa:"
              required
            ></b-form-input>
          </b-form-group>
        </b-col>
      </b-row>

      <b-button type="submit" variant="primary">Submit</b-button>
      <b-button type="reset" variant="danger">Reset</b-button>
    </b-form>
  </div>
</template>

<script>
export default {
  name: "Form",
  data() {
    return {
      form: {
        subject: "",
        description: "",
      },
      foods: [
        { text: "Select One", value: null },
        "Carrots",
        "Beans",
        "Tomatoes",
        "Corn",
      ],
      show: true,
    };
  },
  methods: {},
};
</script>
