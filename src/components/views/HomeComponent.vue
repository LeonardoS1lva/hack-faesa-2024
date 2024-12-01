<template>
  <div>
    <HeaderComponent
      nav1="Login"
      nav2="Cadastro"
      nav3=""
      nav4=""
      link1="#/perfilEmpresa"

    >
      <template #title>
        <img src="../../assets/icons/logo.png" alt="Logo" class="img-logo" />
      </template>
    </HeaderComponent>

    <div class="home-card">
      <CardHome />
    </div>
    <div class="quem-somos">
      <CardSimples
        title="Quem somos?"
        description="Somos uma empresa especializada em terceirização de serviços, comprometida em oferecer soluções eficientes e personalizadas para atender às necessidades dos nossos clientes. Nosso objetivo é simplificar processos, reduzir custos e entregar excelência, permitindo que nossos parceiros foquem no que realmente importa: o crescimento e sucesso do seu negócio."
        width="80%"
      />
    </div>
    <div class="cards-planos">
      <div>
        <h3>Plano Gratuito</h3>
        <ul>
          <li>Visibilidade Limitada dos Leads</li>
          <li>Menor Alcance</li>
          <li>Limite de 3 propostas</li>
          <li>
            Recomendações de cuidados extras em alguns pontos (Análise de Risco)
          </li>
        </ul>
      </div>
      <hr class="line" />
      <div>
        <h3>Plano Premium</h3>
        <ul>
          <li>Destaque nos resultados de busca</li>
          <li>Acesso a todos os Leads</li>
          <li>Propostas ilimitadas</li>
          <li>Impulsionamento de perfil</li>
          <li>
            Recomendações de cuidados extras em alguns pontos (Análise de Risco)
          </li>
        </ul>
      </div>
    </div>
    <div class="ultimo-card">
        <div>
            <h3>Por que terceirizar?</h3>
            <ul>
                <li>Redução de custos: Menos despesas fixas e operacionais.</li>
                <li>Especialização: Serviços realizados por profissionais qualificados.</li>
                <li>Foco no essencial: Mais tempo para atividades estratégicas.</li>
                <li>Flexibilidade: Adaptação rápida às demandas do negócio.</li>
                <li>Eficiência: Melhoria na qualidade e acesso a tecnologia avançada.</li>
            </ul>
        </div>
      <!-- <CardSimples
        title="Por que terceirizar?"
        description="Redução de custos: Menos despesas fixas e operacionais.
Especialização: Serviços realizados por profissionais qualificados.
Foco no essencial: Mais tempo para atividades estratégicas.
Flexibilidade: Adaptação rápida às demandas do negócio.
Eficiência: Melhoria na qualidade e acesso a tecnologia avançada.
"
        width="80%"
      /> -->
    </div>
  </div>
</template>

<script>
import HeaderComponent from "@/components/layouts/Header.vue";
import CardSimples from "../cards/CardSimples.vue";
import CardHome from "../cards/CardHome.vue";

export default {
  components: {
    HeaderComponent,
    CardSimples,
    CardHome,
  },
};
</script>

<style scoped>
.cards-planos {
  display: flex;
  justify-content: center;
  width: 80%;
  margin: 0 auto;
  margin-top: 2rem;
  color: #093047e6;
}

.cards-planos h3 {
    text-align: center;
}

.cards-planos ul {
    display: flex;
    flex-direction: column;
}

.cards-planos div {
    width: 35%;
    padding: 0 1rem;
    display: flex;
    flex-direction: column;
    gap: 0.5rem;
}

.line {
    border: 1px solid #000;
    margin: 0 2rem;
}

.card-home {
    display: flex;
    justify-content: space-between;
    width: 80%;
}

.ultimo-card {
    margin-bottom: 2rem;
    color: #093047e6;
}

.img-logo {
    width: 40px;
  border-radius: 50%;
}

.ultimo-card {
    display: flex;
    justify-content: center;
    gap: 2rem;
    margin-top: 2rem;
}

.ultimo-card h3 {
    text-align: center;
    padding-bottom: 1rem;
}

.ultimo-card ul {
    display: flex;
    flex-direction: column;
    gap: 0.5rem;
}

.ultimo-card ul li {
    list-style: outside;
}
</style>
