<template>
<div>
  <q-table class="data-table-cliente"
    :title="titulo"
    :data="dados"
    :columns="colunas"
    row-key="name"
    :slot="excluir"
    />
</div>

</template>
<script>
import { openURL, QTable, QItemSeparator, QField, QInput, QCard, QCardMain, QItem, QItemTile, QList, QPopover, QToggle, QBtn, QModal } from 'quasar'

export default {
  name: 'DTLojista',
  props: {
    dados: Array,
    colunas: Array,
    titulo: String,
    excluir: String
  },
  data () {
    return {
      name: ''
    }
  },

  components: {
    openURL, QTable, QItemSeparator, QField, QInput, QCard, QItem, QList, QPopover, QToggle, QBtn, QModal, QCardMain, QItemTile
  }

}
</script>
<style>

</style>
