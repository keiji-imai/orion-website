<template>
  <button class="btn-root">
    <slot />
  </button>
</template>

<style lang="postcss" scoped>
.btn-root {
  @apply border-white border-2 p-2 px-4 text-white rounded-tr-lg rounded-bl-lg transition-all relative justify-center items-center flex focus:outline-none;
  background-image: transparent;

  &:hover {
    @apply bg-blue-200 text-black -translate-y-0.5 translate-x-0.5 transform;
    box-shadow: 0 4px 18px 0 theme('colors.blue.400');
  }

  &:active {
    @apply translate-y-0;
  }
}
</style>
