<script setup>
import { defineProps } from 'vue';

const props = defineProps({
  name: String,
  status: String,
  species: String,
  gender: String,
  location: String,
  image: String,
  episodeCount: Number
});
</script>

<template>
    <div class="col-md-4">
        <div class="card mb-3">
            <div class="card">
                <img :src="props.image" class="card-img-top" alt="Imagem do personagem">
            <div class="card-body">
                <h5 class="card-title">{{ props.name }}</h5>
                <p class="card-text"><strong>Status:</strong> {{ props.status }}</p>
                <p class="card-text"><strong>Espécie:</strong> {{ props.species }}</p>
                <p class="card-text"><strong>Gênero:</strong> {{ props.gender }}</p>
                <p class="card-text"><strong>Localização Atual:</strong> {{ props.location }}</p>
                <p class="card-text"><strong>Aparições em Episódios:</strong> {{ props.episodeCount }}</p>
            </div>
            </div>
            
        </div>
    </div>
</template>

<style scoped>

.card {
    border-radius: 5px;
}
.card-body{
    padding-bottom: 35px;
    background-color: #212529;
    color: #fff;
    }
</style>
