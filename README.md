## Teste Técnico Flutter: Aplicativo de Super-Heróis com Múltiplas Abas
 #### Objetivo:
 Desenvolver um aplicativo em Flutter que consome uma API de super-heróis e exibe informações
 em três abas diferentes. Cada aba deve exibir um conjunto distinto de dados e utilizar o Cubit
 para o gerenciamento de estado.
 ##### API: 
 Utilize qualquer API de super-heróis disponível publicamente (como SuperHero API ou
 SuperHeroDB API) para obter informações sobre os heróis.
 #### Requisitos:
 1. Tela de login:
    - O aplicativo deve possuir uma tela de login, onde deve ser solicitado e-mail e senha, também deverá ter um botão para entrar no sistema.
      1. E-mail deverá ser: `teste@teste.com.br`
      2. Senha deverá ser: `teste123`
 2. Interface principal deverá ser composta por 3 Abas:
   - O aplicativo deve conter uma barra de navegação com 3 abas:
     1. Lista de Heróis: Exibir uma lista paginada de heróis (nome, imagem).
     2. Detalhes do Herói: Ao selecionar um herói na aba 'Lista de Heróis', os detalhes desse herói
 (nome, poderes, biografia) devem ser exibidos nesta aba.
     3. Favoritos: Exibir uma lista dos heróis marcados como favoritos pelo usuário.
 3. Funcionalidades para cada aba:
   - Lista de Heróis:
     - Exibir uma lista de super-heróis carregada da API.
     - Implementar paginação para carregar mais heróis ao rolar a lista.
     - O usuário pode clicar em um herói da lista para ver seus detalhes na aba 'Detalhes do Herói'.
   - Detalhes do Herói:
     - Exibir os detalhes completos do herói selecionado na aba anterior.
     - Incluir um botão 'Favoritar' que permite adicionar o herói à lista de favoritos.
   - Favoritos:
     - Exibir uma lista de heróis que foram marcados como favoritos.
     - Cada herói exibido aqui deve ter um botão para ser removido da lista de favoritos.
 4. Gerenciamento de Estado:
   - Implementar um Cubit separado para gerenciar o estado de cada aba.
 5. Lógica de Negócio:
   - O aplicativo deve buscar os dados da API de forma eficiente, com carregamento e tratamento
 de erros.
 6. Validação:
   - Cada Cubit deve gerenciar corretamente o estado de sua aba.

### Avaliação:
  - Uso correto do Cubit para gerenciar o estado de cada aba.
  - Implementação de uma interface clara e funcional.
  - Boas práticas de código e organização.
  - Funcionamento correto da integração com a API e das funcionalidades de favoritos.
    
 ### Pontos Extras:
   - Adicionar animações ao alternar entre as abas (opcional).
   - Implementar um sistema de busca de heróis (opcional).
   - Adicionar testes unitários para os Cubits (opcional).
   - Implementar caching para evitar múltiplas requisições à API (opcional).
