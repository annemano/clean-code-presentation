<template>
  <div class="bg-main slidev-layout">
    <div class="grid grid-cols-2 gap-8" :class="{ 'gap-16': $attrs.reverse }">
      <div
        class="prose pr-16"
        :class="{ 'order-1 text-right': $attrs.reverse }"
      >
        <slot name="default" />
      </div>
      <div class="relative">
        <TheConsole class="rounded-lg shadow-lg object-cover z-10">
          <slot name="window"></slot>
        </TheConsole>
      </div>
    </div>
  </div>
</template>
