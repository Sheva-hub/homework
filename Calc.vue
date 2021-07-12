<template>
  <div>
    <div>
      <input v-model.number="operand1" type="number" placeholder="operand1" />
      <input v-model.number="operand2" type="number" placeholder="operand2" />
      ={{ sum }}
    </div>
    <div>
      <button @click="sum = operand1 + operand2">+</button>
      <button @click="sum = operand1 - operand2">-</button>
      <button @click="sum = operand1 * operand2">*</button>
      <button @click="sum = operand1 / operand2">/</button>
      <button @click="sum = operand1 ** operand2">Возведение в степень</button>
    </div>
  </div>
</template>

<script>
export default {
  name: "Calc",
  data: () => ({
    operand1: 0,
    operand2: 0,
    sum: 0,
  }),
};
</script>

<style>
</style>
