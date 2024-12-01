<template>
  <div>
    <HeaderComponent
      nav1="Início"
      nav2="Perfil"
      nav3="Propostas"
      nav4="Configurações"
      link1="#/"
      link2="#/perfilEmpresa"
      link3="#/resumoPropostas"
    >
      <template #title>
        <img src="../../assets/icons/logo.png" alt="Logo" class="img-logo" />
      </template>
    </HeaderComponent>
  </div>
  <div class="container-propostas">
    <a href="#/buscar">
      <CardSimples
        title="Resumo da sua proposta"
        description="Proposta de licitação de prestação de serviços relacionados à limpeza das áreas comuns do prédio leste entre os meses de novembro e dezembro com o orçamento máximo de R$1.500,00 que atenda as métricas de satisfação dos funcionários e compromisso com o meio ambiente"
        width="80%"
      />
    </a>
    <a href="#/buscar">
      <CardSimples
        title="Resumo da sua proposta"
        description="Proposta de licitação de prestação de serviços relacionados à limpeza das áreas comuns do prédio leste entre os meses de novembro e dezembro com o orçamento máximo de R$1.500,00 que atenda as métricas de satisfação dos funcionários e compromisso com o meio ambiente"
        width="80%"
      />
    </a>
  </div>
</template>

<script>
import HeaderComponent from "@/components/layouts/Header.vue";
import CardSimples from "../cards/CardSimples.vue";

export default {
  components: {
    HeaderComponent,
    CardSimples,
  },
};
</script>

<style scoped>
.img-logo {
  width: 40px;
  border-radius: 50%;
}
a {
  color: #000;
}
</style>
