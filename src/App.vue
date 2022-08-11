<script>
export default {
  data() {
    return {
      words: "",
    };
  },
};
</script>

<template>
  <div class="min-h-screen w-full bg-slate-100 p-12">
    <div class="bg-white flex-1 rounded-xl shadow-xl overflow-hidden">
      <input class="text-5xl font-semibold text-center text-gray-800 py-12 w-full outline-none" v-model="words" />
    </div>
    <ul class="flex flex-wrap gap-12 mt-16">
      <li
        v-for="word in ['Apple', 'Orange', 'Mango', 'Grapes', 'Banana']"
        class="inline-block px-12 py-8 rounded-xl shadow-lg bg-blue-600 text-white text-5xl"
      >
        {{ word }}
      </li>
    </ul>
  </div>
</template>
