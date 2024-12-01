<script setup>
import { ref, computed } from "vue";
import Home from "@/components/views/HomeComponent.vue";
import NotFound from "@/components/views/NotFound.vue";
import TelaBusca from "@/components/views/TelaBusca.vue";
import PerfilEmpresa from "@/components/views/PerfilEmpresa.vue";
import PerfilTerceirizada from "@/components/views/PerfilTerceirizada.vue";
import ResumoPropostas from "@/components/views/ResumoPropostas.vue";
import AvisoContrato from "@/components/views/AvisoContrato.vue";

const routes = {
  "/": Home,
  "/buscar": TelaBusca,
  "/perfilEmpresa": PerfilEmpresa,
  "/perfilTerceirizada": PerfilTerceirizada,
  "/resumoPropostas": ResumoPropostas,
  "/avisoContrato": AvisoContrato,
  "/notFound": NotFound,
};

const currentPath = ref(window.location.hash);

window.addEventListener("hashchange", () => {
  currentPath.value = window.location.hash;
});

const currentView = computed(() => {
  return routes[currentPath.value.slice(1) || "/"] || NotFound;
});
</script>

<template>
  <component :is="currentView" />
</template>
