# 🎙️ Gerenciador de PodCasts

## ℹ️ Descrição 

O **Gerenciador de PodCasts** é uma aplicação que centraliza episódios de podcasts em categorias distintas, inspirada no estilo da Netflix. Seu objetivo é facilitar o acesso e a organização de episódios em formato de vídeo, oferecendo uma navegação intuitiva e agradável.

## 🚀 Funcionalidades

- **Listagem de Episódios por Categoria:** Os episódios são organizados em categorias como saúde, bodybuilder, metodologia ágil, QA, programação e humor, permitindo uma exploração fácil e rápida dos conteúdos.
- **Filtragem de Episódios:** Os usuários podem buscar episódios específicos pelo nome do podcast, simplificando o acesso ao conteúdo desejado.

## ✅ Implementação

### Mensagem de Boas-Vindas

- **Endpoint:** `GET /`
- **Descrição:** Retorna uma mensagem de boas-vindas.
- **Exemplo de Resposta:**

```json
{
  "message": "Seja bem-vindo(a) à API de Gerenciamento de PodCasts"
}
```
# Listar Episódios por Categoria
Endpoint: GET /api/list
Descrição: Retorna uma lista de episódios organizados por categorias.
Exemplo de Resposta:

Filtrar Episódios por Nome de Podcast
Endpoint: GET /api/podcasts?p={nome}
Descrição: Retorna episódios com base no nome do podcast fornecido.
Exemplo de Requisição: GET /api/podcasts?p=flow

## 💻 Tecnologias Utilizadas
TypeScript: Linguagem de programação utilizada para desenvolvimento.
Tsup: Ferramenta para construção e empacotamento de projetos TypeScript.
Tsx: Compilador TypeScript que suporta a construção de projetos.
Node.js: Ambiente de execução JavaScript no lado do servidor.
@types/node: Pacote de definições de tipos para Node.js, auxiliando no desenvolvimento com TypeScript.

## 📝 Como Utilizar
Clone este repositório: https://github.com/ronaldohauser/api-gerenciador-podcast.
Instale as dependências: npm install.
Inicie o servidor: npm run start:dev.
Acesse os endpoints para listar ou filtrar episódios de podcasts.
