<template>
  <div>
    <div class="groups">
      <div
        class="group"
        v-for="group in groups"
        :key="group._id"
      >
        {{ group.name }}
        <b-table
          hover
          simple
          :items="group.items"
          :fields="fields"
        >
        </b-table>
      </div>
    </div>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'

export default Vue.extend({
  data () {
    return {
      fields: [{
        key: 'name',
        label: 'Nome',
        sortable: true
      }],
      groups: [{
        _id: 'group1',
        name: 'Grupo 1',
        items: [
          { name: 'Abobrinha' },
          { name: 'Acelga' },
          { name: 'Agrião' },
          { name: 'Aipo' },
          { name: 'Alface' },
          { name: 'Almeirão' },
          { name: 'Brócolis' },
          { name: 'Chicória' },
          { name: 'Couve' },
          { name: 'Escarola' },
          { name: 'Espinafre' },
          { name: 'Nabo' },
          { name: 'Pepino' },
          { name: 'Pimentão' },
          { name: 'Rabanete' },
          { name: 'Repolho' },
          { name: 'Rúcula' },
          { name: 'Salsão' },
          { name: 'Tomate' }
        ]
      }, {
        _id: 'group2',
        name: 'Grupo 2',
        items: [
          { name: 'Abóbora' },
          { name: 'Aspargo' },
          { name: 'Beringela' },
          { name: 'Beterraba' },
          { name: 'Cenoura' },
          { name: 'Chuchu' },
          { name: 'Cogumelo' },
          { name: 'Couve flor' },
          { name: 'Ervilha' },
          { name: 'Palmito' },
          { name: 'Quiabo' },
          { name: 'Vagem' }
        ]
      }, {
        _id: 'group3',
        name: 'Grupo 3',
        items: [
          { name: 'Abacaxi - 1 rodela pequena' },
          { name: 'Acerola - 1 pequena' },
          { name: 'Água de coco - 1 copo pequeno' },
          { name: 'Ameixa - 2 médias' },
          { name: 'Amora - meio copo' },
          { name: 'Banana - 1 pequena' },
          { name: 'Caju - 1 médio' },
          { name: 'Caqui - 1 pequeno' },
          { name: 'Carambola - 1 média' },
          { name: 'Cereja - 6 frutas' },
          { name: 'Damasco - 2 médios' },
          { name: 'Figo - 1 médio' },
          { name: 'Framboesa - 10 frutas' },
          { name: 'Goiaba - 1 pequena' },
          { name: 'Jabuticaba - 10 frutas' },
          { name: 'Kiwi - 1 médio' },
          { name: 'Laranja - 1 pequena' },
          { name: 'Maça - 1 média' },
          { name: 'Mamão - 1 fatia pequena' },
          { name: 'Manga - 1 pequena' },
          { name: 'Maracujá - 1 pequeno' },
          { name: 'Melancia - 1 fatia média' },
          { name: 'Morango - 10 frutas' },
          { name: 'Melão - 1 fatia pequena' },
          { name: 'Nectarina - 1 média' },
          { name: 'Pêra - 1 pequena' },
          { name: 'Pêssego - 1 médio' },
          { name: 'Salada de frutas - 3 colheres de sopa' },
          { name: 'Tangerina - 1 média' },
          { name: 'Uva passa - 1 colher de sopa' },
          { name: 'Uva - 10 frutas' }
        ]
      }, {
        _id: 'group4',
        name: 'Grupo 4',
        items: []
      }, {
        _id: 'group5',
        name: 'Grupo 5',
        items: []
      }, {
        _id: 'group6',
        name: 'Grupo 6',
        items: []
      }, {
        _id: 'group7',
        name: 'Grupo 7',
        items: []
      }, {
        _id: 'group8',
        name: 'Grupo 8',
        items: []
      }]
    }
  }
})
</script>

<style scoped>
.groups {
  display: flex;
  justify-content: space-between;
  height: 25vh;
  overflow: hidden;
}
.groups .group {
  overflow: auto;
}
</style>
