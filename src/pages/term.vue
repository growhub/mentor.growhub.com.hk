<template>
  <div>
    <breadcrumb
      :breadcrumbs="[
        { to: '/', label: 'HOME' },
        { to: '/term', label: 'Term' }
      ]"
    />
    <term-section />
  </div>
</template>

<script lang="ts">
import { createComponent } from '@vue/composition-api'
import Breadcrumb from '~/components/molecules/Breadcrumb.vue'
import TermSection from '~/components/organisms/term/TermSection.vue'

export default createComponent({
  components: {
    Breadcrumb,
    TermSection
  }
})
</script>
