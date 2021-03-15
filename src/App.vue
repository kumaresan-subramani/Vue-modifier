<template>
  <div id="app">
    
    <h6>Controls with .lazy modifier</h6>
    <div>
      <h4>Syncfusion Textbox</h4>
      <ejs-textbox
        v-model.lazy="textboxvalue"
        placeholder="Focus and click enter"
      ></ejs-textbox>
      <p>Textbox value is: {{ textboxvalue }}</p>
    </div>
    <div>
      <h4>Native Textbox</h4>
      <input v-model.lazy="msg" />
      <p>Native Textbox value is: {{ msg }}</p>
    </div>
  </div>
</template>

<script>
import Vue, { VueConstructor } from "vue";
import { DatePickerPlugin } from "@syncfusion/ej2-vue-calendars";
import { ButtonPlugin } from "@syncfusion/ej2-vue-buttons";
import {
  TextBoxPlugin,
  NumericTextBoxPlugin,
} from "@syncfusion/ej2-vue-inputs";
Vue.use(TextBoxPlugin);
Vue.use(NumericTextBoxPlugin);
Vue.use(ButtonPlugin);
Vue.use(DatePickerPlugin);

export default Vue.extend({
  data() {
    return {
      textboxvalue: "Syncfusion",
      numericvalue: 10,
      Inputnumber: 21,
      msg: "Textbox",
      textboxInput: "Hi World",
      textboxvalue1: "Syncfusion1",
      numericvalue1: 11,
      inputNumer1: 22,
      msg1: "Textbox1",
      textboxInput1: "Hi",
    };
  },
});
</script>

<style lang="scss">
@import "../node_modules/@syncfusion/ej2-base/styles/material.css";
@import "../node_modules/@syncfusion/ej2-buttons/styles/material.css";
@import "../node_modules/@syncfusion/ej2-inputs/styles/material.css";
@import "../node_modules/@syncfusion/ej2-popups/styles/material.css";
@import "../node_modules/@syncfusion/ej2-vue-buttons/styles/material.css";
@import "../node_modules/@syncfusion/ej2-vue-calendars/styles/material.css";
@import "../node_modules/@syncfusion/ej2-vue-inputs/styles/material.css";
</style>
