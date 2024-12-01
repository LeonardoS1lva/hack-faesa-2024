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
      <CardPerfilTerceirizada width="80%" />
    </div>
    <div class="cards">
      <CardSimples
        title="Missão e Valores"
        description="Proporcionar ambientes limpos, seguros e saudáveis, garantindo bem-estar e produtividade para nossos clientes, com responsabilidade social e ambiental."
        width="49%"
      />
      <CardSimples
        title="Qualidades e diferenciais"
        description="Profissionais Capacitados;
Soluções Personalizadas; Sustentabilidade;
Tecnologia de Ponta;
Atendimento Ágil e Humanizado;"
        width="49%"
      />
    </div>
    <div class="container-3cards">
      <CardSimples
        title="Licenças e certidões"
        description="Alvará de funcionamento válido;
Certificado de Regularidade junto ao INSS e FGTS;
Registro no Cadastro Técnico Federal (CTF/IBAMA);
Licença ambiental para descarte correto de resíduos;
Certificação ISO 9001 (Gestão da Qualidade);"
        width="32%"
      />
      <CardSimples
        title="Capacidade técnica"
        description="Equipe composta por 50 colaboradores especializados em limpeza;
Frota própria de veículos para transporte de equipamentos e produtos;
Ferramentas avançadas para limpeza de fachadas, pisos industriais, carpetes, vidros e sanitização de ambientes;"
        width="32%"
      />
      <CardSimples
        title="Capacidade de atuação"
        description="Atendimento a empresas de pequeno, médio e grande porte, incluindo hospitais, indústrias, escolas, shopping centers e condomínios."
        width="32%"
      />
    </div>
    <div class="principios">
      <CardSimples
        title="Relatórios e avaliações"
        description=""
        width="100%"
      />
    </div>
  </div>
</template>

<script>
import HeaderComponent from "@/components/layouts/Header.vue";
import CardSimples from "@/components/cards/CardSimples.vue";
import CardPerfilTerceirizada from "@/components/cards/CardPerfilTerceirizada.vue";

export default {
  components: {
    HeaderComponent,
    CardSimples,
    CardPerfilTerceirizada,
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
  width: 80%;
  margin: 0 auto;
  margin-bottom: 2rem;
}

.container-3cards {
  display: flex;
  justify-content: space-between;
  width: 80%;
  margin: 0 auto;
}

.img-logo {
  width: 40px;
  border-radius: 50%;
}
</style>
