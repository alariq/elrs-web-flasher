<script setup>
import {hasFeature, store} from "../js/state.js";

</script>

<template>
  <VTextField v-model="store.options.cf.freqStart" label='Start Freq:'/>
  <VTextField v-model="store.options.cf.freqEnd" label='End Freq:'/>
</template>
