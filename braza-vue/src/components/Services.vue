<template>
    <div id="services">
      <h2>Como nós trabalhamos</h2>
      <div id="grade-services">
        <div class="caixa-service" v-for="(service, index) in services" :key="index">
          <div class="linha-caixa">
            <img :src="service.image" class="imagem-caixa" :alt="service.title" />
            <h3>{{ service.title }}</h3>
          </div>
          <p>{{ service.description }}</p>
          <a :href="service.link">
            <button class="botao-caixa">
              Saiba mais<i class="fas fa-arrow-right"></i>
            </button>
          </a>
        </div>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    data() {
      return {
        services: [
          {
            image: '@/assets/pagina-da-internet.png',
            title: 'Criação de site',
            description: 'Destaque-se online com um site único e envolvente...',
            link: 'https://wa.me/5582999355730',
          },
          // Adicione os outros serviços aqui
        ],
      };
    },
  };
  </script>
  
  <style scoped>
  /* Estilos da seção Serviços */
  </style>
  