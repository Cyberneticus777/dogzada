<script>
import CachorroCard from '@/components/cachorrada/CachorroCard.vue'

export default {
  components: { CachorroCard },
  data() {
    return {
      cachorros: [
        {id: 1, nome: 'Reis 1'},
        {id: 2, nome: 'Reis 2'},
        {id: 3, nome: 'Reis 3'},
        {id: 4, nome: 'Reis 4'},
        {id: 5, nome: 'Reis 5'},
      ]
    }
  }
}
</script>
<template>
    <div class="card-group">
      <CachorroCard v-for="cachorro in cachorros" :key="cachorro.id" :cachorro="cachorro" />
    </div>
</template>

<style>

</style>
