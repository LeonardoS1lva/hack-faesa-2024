<template>
    <div class="card">
      <div class="container">
        <div class="container-1">
          <h4>
            <b>{{ title }}</b>
          </h4>
          <ul>
            <li>Preço oferecido: R$ 1.000,00</li>
            <li>Serviço Oferecido: Limpeza</li>
            <li>Tempo médio: 10 meses</li>
            <li>Localidade: Vitória</li>
          </ul>
        </div>
        <div class="container-2">
          <h5>Selos</h5>
          <div class="container-selos">
            <img :src="icon1" alt="icone" />
            <img :src="icon2" alt="icone" />
          </div>
          <a href="#/perfilTerceirizada">
              <button>Saiba mais</button>
          </a>
        </div>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    props: {
      title: {
        type: String,
        required: true,
      },
      icon1: {
        type: String,
        required: true,
      },
      icon2: {
        type: String,
        required: true,
      },
    },
  };
  </script>
  
  <style scoped>
  .card {
    /* background-color: #d9d9d9; */
    background: linear-gradient(285deg, rgba(16, 69, 99, 0.90) 3.74%, rgba(5, 45, 67, 0.89) 52.63%, #032030 101.8%);
  color: #fff;
    padding: 1rem;
    margin-top: 2rem;
    border-radius: 1.5rem;
  }
  
  .container {
    display: flex;
  }
  
  .container-1 {
      display: flex;
      flex-direction: column;
      padding: 0 3rem;
      gap: 0.5rem;
  }
  
  .container-1 ul {
      display: flex;
      flex-direction: column;
      padding: 0 1rem;
  }
  
  .container-2 {
      display: flex;
      flex-direction: column;
      padding: 0 1rem;
      gap: 0.5rem;
  }
  
  .container-2 h5 {
      text-align: center;
  }
  
  .container-selos {
      display: flex;
      justify-content: center;
      gap: 1rem;
  }
  
  li {
      list-style: outside;
  }
  
  button {
      background-color: #fff;
      color: #000;
      font-weight: bold;
      border: none;
      border-radius: 5px;
      padding: 0.5rem 1rem;
      margin-top: 1rem;
  }
  
  button:hover {
      background-color: #c0c0c0;
      cursor: pointer;
  }
  </style>
  