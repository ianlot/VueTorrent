<template>
  <v-flex xs6 sm2>
    <div class="caption grey--text">
      {{ $t('torrent.properties.completed_on') | titleCase }}
    </div>
    <div>{{ torrent.completed_on }}</div>
  </v-flex>
</template>

<script lang="ts">
import { defineComponent } from 'vue'
import { TorrentDashboardItem } from '@/mixins'

export default defineComponent({
  name: 'CompletedOn',
  mixins: [TorrentDashboardItem]
})
</script>
