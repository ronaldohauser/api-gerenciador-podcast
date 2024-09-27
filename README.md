# 🎙️ Gerenciador de PodCasts

## ℹ️ Descrição 

O **Gerenciador de PodCasts** é uma aplicação que centraliza episódios de podcasts em diferentes categorias, inspirada no estilo da Netflix. O objetivo é facilitar o acesso e a organização de episódios em formato de vídeo, proporcionando uma navegação intuitiva e agradável.

## 🚀 Funcionalidades

- **Listagem de episódios por categoria:** Os episódios são organizados em categorias como saúde, bodybuilder, metodologia ágil, QA, programação e humor, permitindo fácil exploração dos conteúdos.
- **Filtragem de episódios:** Os usuários podem buscar episódios específicos pelo nome do podcast, simplificando o acesso ao conteúdo desejado.

## ✅ Implementação

### Mensagem de Boas-Vindas

- **Endpoint:** `GET /`
- **Descrição:** Retorna uma mensagem de boas-vindas.
- **Exemplo de resposta:**

```json
{
  "message": "Seja bem-vindo(a) à API de Gerenciamento de PodCasts"
}
Listar Episódios por Categoria
Endpoint: GET /api/list
Descrição: Retorna uma lista de episódios organizados por categorias.
Exemplo de resposta:
json
Copiar código
[
    {
      "podcastName": "flow",
      "episode": "SCRUM MASTER - Flow #320",
      "videoId": "4KDGTdiOV4I",
      "categories": ["metodologia ágil", "programação"]
    },
    {
      "podcastName": "flow",
      "episode": "QUALIDADE DE SOFTWARE - Flow #321",
      "videoId": "4KDGTdiOA4I",
      "categories": ["qa", "programação"]
    }
]
Filtrar Episódios por Nome de Podcast
Endpoint: GET /api/podcasts?p={nome}
Descrição: Retorna episódios com base no nome do podcast fornecido.
Exemplo de requisição: GET /api/podcasts?p=flow
💻 Tecnologias Utilizadas
TypeScript: Linguagem de programação para desenvolvimento.
Tsup: Ferramenta para construção e empacotamento de projetos TypeScript.
Tsx: Compilador TypeScript que suporta construção de projetos.
Node.js: Ambiente de execução JavaScript para o lado do servidor.
@types/node: Pacote de definições de tipos para Node.js, auxiliando no desenvolvimento com TypeScript.
📝 Como Utilizar
Clone este repositório: https://github.com/ronaldohauser/api-gerenciador-podcast.
Instale as dependências: npm install.
Inicie o servidor: npm run start:dev.
Acesse os endpoints para listar ou filtrar episódios de podcasts.