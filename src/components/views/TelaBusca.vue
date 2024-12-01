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
    <Card
      title="Resumo de sua proposta"
      description="Proposta de licitação de prestação de serviços relacionados à limpeza das áreas comuns do prédio leste entre os meses de novembro e dezembro com o orçamento máximo de R$1.500,00 que atenda as métricas de satisfação dos funcionários e compromisso com o meio ambiente"
    />
    <div class="containerEmpresa">
      <CardEmpresa
        title="Empresa 1"
        icon1="src/assets/icons/mao.png"
        icon2="src/assets/icons/money.png"
      />
      <CardEmpresa
        title="Empresa 2"
        icon1="src/assets/icons/cerebro.png"
        icon2="src/assets/icons/terra.png"
      />
    </div>
    <a href="#/">
        <button>Descubra mais</button>
    </a>
  </div>
</template>

<script>
import HeaderComponent from "@/components/layouts/Header.vue";
import Card from "@/components/cards/CardProposta.vue";
import CardEmpresa from "@/components/cards/CardEmpresa.vue";

export default {
  components: {
    HeaderComponent,
    Card,
    CardEmpresa,
  },
};
</script>

<style scoped>
.containerEmpresa {
  display: flex;
  justify-content: space-between;
  width: 80%;
  margin: 0 auto;
}
button {
  background-color: #333;
  color: #fff;
  font-weight: bold;
  border: none;
  border-radius: 1rem;
  padding: 1rem 2rem;
  margin: 2rem auto;
  display: block;
}

button:hover {
  background-color: #333333cc;
  cursor: pointer;
}

.img-logo {
  width: 40px;
  border-radius: 50%;
}
</style>
