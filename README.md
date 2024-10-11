# Teste Técnico Flutter: Aplicativo de Super-Heróis

## Objetivo:
Desenvolver um aplicativo em Flutter que consome uma API de super-heróis e exibe informações em três abas diferentes. 
Cada aba deve exibir um conjunto distinto de dados e utilizar um Cubit separado para o gerenciamento de estado.

## API:
Utilize qualquer API de super-heróis disponível publicamente (como SuperHero API ou SuperHeroDB API) para obter informações sobre os heróis.

## Requisitos:

### 1. Tela de login
- O aplicativo deve possuir uma tela de login, onde deve ser solicitado e-mail e senha, também deverá ter um botão para entrar no sistema
  1. **E-mail**: Validar para somente autenticar com o e-mail `teste@teste.com.br`
  2. **Senha**: Validar para somente autenticar com a senha `teste123`

### 1. Tela principal com 3 abas:
- O aplicativo deve conter uma barra de navegação com 3 abas:
  1. **Lista de Heróis**: Exibir uma lista paginada de heróis (nome, imagem).
  2. **Detalhes do Herói**: Ao selecionar um herói na aba "Lista de Heróis", os detalhes desse herói (nome, poderes, biografia) devem ser exibidos nesta aba.
  3. **Favoritos**: Exibir uma lista dos heróis marcados como favoritos pelo usuário.

### 2. Funcionalidades para cada aba:
- **Lista de Heróis**:
  - Exibir uma lista de super-heróis carregada da API.
  - Implementar paginação para carregar mais heróis ao rolar a lista.
  - O usuário pode clicar em um herói da lista para ver seus detalhes na aba "Detalhes do Herói".
  
- **Detalhes do Herói**:
  - Exibir os detalhes completos do herói selecionado na aba anterior.
  - Dados exibidos devem incluir: nome, descrição, poderes, estatísticas de combate (força, velocidade, etc.).
  - Incluir um botão "Favoritar" que permite adicionar o herói à lista de favoritos.
  
- **Favoritos**:
  - Exibir uma lista de heróis que foram marcados como favoritos.
  - Cada herói exibido aqui deve ter um botão para ser removido da lista de favoritos.

### 3. Gerenciamento de Estado:
- Implementar um **Cubit** separado para gerenciar o estado de cada aba:
  - **Lista de Heróis Cubit**: Gerencia a lista paginada de heróis.
  - **Detalhes do Herói Cubit**: Gerencia os detalhes do herói selecionado.
  - **Favoritos Cubit**: Gerencia a lista de heróis favoritos.
- O estado de cada aba deve ser mantido ao alternar entre elas.

### 4. Lógica de Negócio:
- O aplicativo deve buscar os dados da API de forma eficiente, com carregamento e tratamento de erros.
- A navegação entre as abas deve ser suave, e o estado de cada aba deve ser mantido.
- Os dados dos heróis devem ser exibidos com uma interface simples e visualmente agradável.
- A lista de heróis favoritos deve ser persistida, ou seja, ao fechar o aplicativo e reabri-lo, os heróis marcados como favoritos devem continuar na lista.

### 5. Validação:
- Cada Cubit deve gerenciar corretamente o estado de sua aba.
- O estado das abas deve ser mantido mesmo ao alternar entre elas.
- O uso correto da API, incluindo o tratamento de erros e a paginação na aba "Lista de Heróis".
- A lista de favoritos deve funcionar corretamente, com a adição e remoção de heróis.

## Avaliação:
- Uso correto do **Cubit** para gerenciar o estado de cada aba (preferencialmente um arquivo para cada aba).
- Implementação de uma interface clara e funcional, com navegação suave entre as abas.
- Boas práticas de código, organização, e modularidade.
- Funcionamento correto da integração com a API de super-heróis (carregamento de dados, tratamento de erros).
- Funcionamento correto da funcionalidade de favoritar heróis, com persistência.

## Pontos Extras:
- Adicionar animações ao alternar entre as abas.
- Implementar um sistema de busca de heróis na aba "Lista de Heróis".
- Adicionar testes unitários.
- Adicionar testes de Widgets.
- Implementar caching para evitar múltiplas requisições à API.
