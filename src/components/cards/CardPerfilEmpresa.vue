<template>
  <div class="card" :style="{ width: width }">
    <div class="container-dados">
      <img
        src="../../assets/icons/company.png"
        alt="logo"
        class="logo-empresa"
      />
      <div class="dados-empresa">
        <h3>EMPRESA CONTRATANTE</h3>
        <p>RAMO DE ATUAÇÃO: Terceirização de serviços empresariais</p>
        <p>CNPJ: 23.423.543/0001</p>
        <p>⭐⭐⭐⭐⭐</p>
        <p>Nosso site</p>
      </div>
    </div>
    <div class="selos">
      <h5>Selos e premiações</h5>
      <div class="selos-icons">
        <img src="../../assets/icons/mao.png" alt="selo" />
        <img src="../../assets/icons/money.png" alt="selo" />
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    width: {
      type: String,
    },
  },
};
</script>

<style>
.card {
  /* background-color: #d9d9d9; */
  background: linear-gradient(
    285deg,
    rgba(16, 69, 99, 0.9) 3.74%,
    rgba(5, 45, 67, 0.89) 52.63%,
    #032030 101.8%
  );
  color: #fff;
  padding: 1rem;
  border-radius: 1.5rem;
  display: flex;
  justify-content: space-around;
  margin: 0 auto;
  margin-top: 2rem;
  box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2);
}
.dados-empresa {
  display: flex;
  flex-direction: column;
  gap: 0.5rem;
}

.selos {
  display: flex;
  flex-direction: column;
  gap: 0.5rem;
}

.selos-icons {
  display: flex;
  gap: 0.5rem;
}

.logo-empresa {
  width: 100px;
  height: 100px;
  border: 2px solid #fff;
  border-radius: 50%;
  align-self: center;
}

.container-dados {
  display: flex;
  gap: 1rem;
}
</style>
