<script setup>
import { ref } from "vue";
const title = "Task List";
// function login(event) {
//   alert("Login button clicked!");
// }
const message = ref("Please login to continue.");
console.log(message);
function login(event) {
  event.preventDefault(); // Prevent the default form submission behavior
  message.value = "Welcome! You have successfully logged in.";
}
</script>

<template>
  <main class="flex min-h-screen items-center justify-center bg-slate-100 p-4">
    <!-- <form
       @submit="login" 
      class="w-full max-w-sm space-y-4 rounded-2xl bg-white p-8 shadow"
    > -->
    <form class="w-full max-w-sm space-y-4 rounded-2xl bg-white p-8 shadow">
      <h1 class="text-2xl font-bold text-brand">
        <i class="bi bi-check2-square"></i> {{ title }} <br />
        <span class="text-sm font-normal text-slate-500">
          {{ message }}
        </span>
      </h1>
      <label class="block">
        E-mail
        <input type="email" class="mt-1 w-full rounded-lg border px-3 py-2" />
      </label>
      <label class="block">
        Parolă
        <input
          type="password"
          class="mt-1 w-full rounded-lg border px-3 py-2"
        />
      </label>
      <!-- <button
        type="submit"
        class="w-full rounded-lg bg-brand py-2 font-semibold text-white"
      > -->
      <button
        @click="login"
        class="w-full rounded-lg bg-brand py-2 font-semibold text-white"
      >
        Intră
      </button>
    </form>
  </main>
</template>

<style scoped></style>
