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
    <div>
      <CardPerfilEmpresa width="80%" />
    </div>
    <div class="cards">
      <CardSimples
        title="Missão e Valores"
        description="Facilitar conexões estratégicas e confiáveis entre empresas e prestadores de serviços terceirizados, promovendo soluções personalizadas e de alta qualidade que impulsionem a eficiência e o sucesso dos nossos clientes."
        width="49%"
      />
      <CardSimples
        title="Quem somos?"
        description="Somos uma empresa especializada em conectar negócios a soluções terceirizadas de alta qualidade. Nosso propósito é simplificar e otimizar o processo de seleção de prestadores de serviços, ajudando empresas a encontrar parceiros ideais que atendam às suas demandas com eficiência, confiabilidade e inovação."
        width="49%"
      />
    </div>
    <div class="principios">
      <!-- <CardSimples
        title="Princípios da empresa"
        description="1 - loren ipsum dolor sit amet, consectetur adipiscing elit. Nullam nec purus nec eros tincidunt aliquam. Nullam nec purus nec eros tincidunt aliquam. Nullam nec purus nec eros 2 - loren ipsum dolor sit amet, consectetur adipiscing elit. Nullam nec purus nec eros"
        width="100%"
      /> -->
      <div>
        <h3>Princípios da empresa</h3>
        <ul>
          <li>Excelência em Parcerias</li>
          <li>Ética e Transparência</li>
          <li>Foco no Cliente</li>
          <li>Inovação Contínua</li>
        </ul>
      </div>
    </div>
  </div>
</template>

<script>
import HeaderComponent from "@/components/layouts/Header.vue";
import CardSimples from "@/components/cards/CardSimples.vue";
import CardPerfilEmpresa from "@/components/cards/CardPerfilEmpresa.vue";

export default {
  components: {
    HeaderComponent,
    CardSimples,
    CardPerfilEmpresa,
  },
};
</script>

<style scoped>
.cards {
  display: flex;
  justify-content: space-between;
  width: 80%;
  margin: 0 auto;
}

.principios {
  display: flex;
  justify-content: space-between;
  width: 79%;
  margin: 0 auto;
  background: linear-gradient(
    285deg,
    rgba(16, 69, 99, 0.9) 3.74%,
    rgba(5, 45, 67, 0.89) 52.63%,
    #032030 101.8%
  );
  padding: 20px;
  border-radius: 1.5rem;
  margin-top: 2rem;
  color: #fff;
  padding-left: 3rem;
}

.img-logo {
  width: 40px;
  border-radius: 50%;
}

.principios li {
  list-style: outside;
}

.principios ul {
  display: flex;
  flex-direction: column;
  gap: 0.5rem;
}
</style>
