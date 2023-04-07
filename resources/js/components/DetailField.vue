<template>
  <PanelItem :index="index" :field="field">
    <template #value>
      <Excerpt :content="field.value" :should-show="false"/>
    </template>
  </PanelItem>
</template>

<script setup>
import {onMounted} from 'vue'

const props = defineProps({
  index: {
    required: true
  },
  resource: {
    required: true
  },
  resourceName: {
    required: true
  },
  resourceId: {
    required: true
  },
  field: {
    required: true
  },
})

onMounted(() => {

})
</script>
