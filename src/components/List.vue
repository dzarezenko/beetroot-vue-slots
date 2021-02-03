<template>
  <div>
    <ol>
      <li v-for="(i, j) in 10" :key="i">
        <slot name="listItem" :counter="i" :counter1="j">
          Item {{ i }} / {{ j }}
        </slot>
      </li>
    </ol>
  </div>
</template>
