<template>
  <div>
    <navbar />
    <Nuxt keep-alive />
    <footer class="mt-16 flex justify-between px-4 md:px-16 items-center h-12 shadow-inner">
      <div class="text-gray-700">
        <a href="/admin">Members</a> |
        <nuxt-link to="/contributing">Guide</nuxt-link>
      </div>
      <p class="text-sm text-gray-900">© Global Alliance for Peace 2020</p>
    </footer>
  </div>
</template>

<style lang="postcss">
:root {
  --primary: #07a6de4e;
}
footer a:hover {
  @apply text-blue-600;
}
.container {
  @apply max-w-4xl mx-auto px-4;
}
h1 + p {
  @apply text-lg;
}

h2 {
  @apply text-2xl;
}

section h2,
h1 {
  @apply text-5xl tracking-tighter max-w-4xl;
}
.page h2 {
  @apply pb-2;
}
.page h2:not(:first-child) {
  @apply pt-6;
}
.page p,
.page h2 {
  @apply max-w-xl;
}
section {
  @apply pt-16;
}
h3 {
  @apply text-lg;
}

h4,
li h3 {
  @apply text-xl;
}

ul + p a,
a.list {
  @apply text-blue-600 font-bold;
  display: inline-block;
  text-transform: uppercase;
}

ul + p a:hover,
a.list:hover {
  padding-right: 1.6rem;
  text-decoration: underline;
}

p,
.page ul {
  @apply max-w-2xl;
}

.rounded-xs {
  border-radius: 2px;
}

table {
  margin-left: -1rem;
}

th {
  text-align: left;
}
th,
td {
  padding-left: 1rem;
}
</style>