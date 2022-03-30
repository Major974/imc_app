<template>
  <div>
    <form @submit.prevent="handleSubmit">
      <label for="taille"> taille </label>
      <input
        type="number"
        v-model="taille"
        name="taille"
        id="taille"
        placeholder="taille"
      />
      <label for="poids"> poids </label>
      <input
        type="number"
        name="poids"
        id="poids"
        v-model="poids"
        placeholder="poids"
      />
      <input type="submit" value="Calculer" />
    </form>
  </div>

  <br />

  <table>
    <thead>
      <tr>
        <th scope="col"></th>
        <th scope="col">taille</th>
        <th scope="col">poids</th>
        <th scope="col">masse corporelle</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td>{{ taille }}</td>
        <td>{{ poids }}</td>
        <td>{{ total }}</td>
      </tr>
      <tr></tr>
    </tbody>
  </table>
</template>

<script setup lang="ts">

</script>

<style></style>
