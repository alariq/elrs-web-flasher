<script setup>
import {hasFeature, store} from "../js/state.js";

defineProps(['type' ])

function is_high_only() {
  return store.radio && store.radio.endsWith('2400')
}

function is_low_only() {
  return store.radio && store.radio.endsWith('900')
}

function is_dual() {
  return store.radio && store.radio.endsWith('dual')
}
</script>

<template>
  <VCard>
    <VCardTitle v-if="is_low_only() || is_dual()">{{ type }} Band: subGHz (a.k.a. 915MHz)</VCardTitle>
    <VCardTitle v-if="is_high_only()">{{ type }} Band: 2G4 (a.k.a 2.4GHz)</VCardTitle>
    <VTextField v-model="store.options.cf.freqStart" label='Start Freq:'/>
    <VTextField v-model="store.options.cf.freqEnd" label='End Freq:'/>
  </VCard>
  <br>
  <template v-if="is_dual()">
  <VCard>
    <VCardTitle>Secondary Band: 2G4 (a.k.a. 2.4GHz)</VCardTitle>
    <VTextField v-model="store.options.cf.freqSecStart" label='Start Freq:'/>
    <VTextField v-model="store.options.cf.freqSecEnd" label='End Freq:'/>
  </VCard>
  <br>
  </template>
</template>
