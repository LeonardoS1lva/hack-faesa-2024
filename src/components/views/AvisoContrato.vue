<template>
  <div>
    <HeaderComponent
      nav1="Início"
      nav2="Perfil"
      nav3="Propostas"
      nav4="Configurações"
      link1="/"
      link2="/perfilEmpresa"
      link3="/resumoPropostas"
    >
      <template #title>
        <img src="../../assets/icons/logo.png" alt="Logo" class="img-logo" />
      </template>
    </HeaderComponent>
    <CardSimples title="Atente-se a esses pontos:" description="" width="90%" />

    <div class="card-aviso">
      <h3>
        Você está contratando uma empresa de forncecimento de serviços de
        limpeza.
      </h3>
      <ul>
        <li>
          Está havendo um debate entre o legislátivo para regulamentar o uso de
          certos solventes.
        </li>
        <li>
          Iniciou-se uma discussão no plenário sobre a discussão para reduzir a
          carga de horária de 6x1 para 5x2.
        </li>
      </ul>
      <p>Verifique se esses pontos podem impactar, e como, o seu contrato.</p>
      <button>Veja mais</button>
    </div>
  </div>
</template>

<script>
import CardSimples from "../cards/CardSimples.vue";
import HeaderComponent from "../layouts/Header.vue";

export default {
  components: {
    CardSimples,
    HeaderComponent,
  },
};
</script>

<style scoped>
.img-logo {
  width: 40px;
  border-radius: 50%;
}

.card-aviso {
  width: 90%;
  margin: 0 auto;
  padding: 20px;
  border: 1px solid #ccc;
  border-radius: 1.5rem;
  background: linear-gradient(285deg, rgba(16, 69, 99, 0.90) 3.74%, rgba(5, 45, 67, 0.89) 52.63%, #032030 101.8%);
  margin-top: 2rem;
  color: #fff;
}

.card-aviso ul {
  list-style: outside;
  display: flex;
  flex-direction: column;
  padding: 1rem;
}

.card-aviso button {
  background-color: #fff;
  color: #000;
  font-weight: bold;
  border: none;
  border-radius: 1rem;
  padding: 1rem 2rem;
  margin: 2rem auto;
  display: block;
}

.card-aviso button:hover {
  background-color: #c0c0c0;
  cursor: pointer;
}
</style>
