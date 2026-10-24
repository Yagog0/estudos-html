# Estudos de desenvolvimento web

![HTML](https://img.shields.io/badge/HTML-E34F26?logo=html5&logoColor=white)
![CSS](https://img.shields.io/badge/CSS-1572B6?logo=css&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?logo=javascript&logoColor=black)
![Node.js](https://img.shields.io/badge/Node.js-339933?logo=nodedotjs&logoColor=white)

Projetos de estudo de **Yago Maba**, com interfaces web e comunicação em tempo real.

## Projetos

| Pasta | Projeto | Tecnologias |
| --- | --- | --- |
| [Página de apresentação](<Pagina Basica de apresentação/>) | Portfólio pessoal com apresentação e interesses | HTML e CSS |
| [Chat de conversa](<chat de conversa/>) | Chat que distribui mensagens entre clientes conectados | HTML, CSS, JavaScript, Node.js e WebSocket |

O diretório do chat também contém um exercício simples de soma em C++ (`calculadora.cpp`) e uma cópia da interface na raiz. A interface usada abaixo fica em `frontend/`.

## Abrir o portfólio

Abra `Pagina Basica de apresentação/index.html` no navegador. As imagens estão na subpasta `imagens/`.

## Executar o chat localmente

Requisitos: Node.js com npm e um navegador.

```sh
cd "chat de conversa/backend"
npm ci
npm start
```

Mantenha o servidor em execução e abra `chat de conversa/frontend/index.html` em duas abas. A interface conecta ao WebSocket em `ws://localhost:8080`; as mensagens são retransmitidas aos clientes conectados.

O backend aceita a variável de ambiente `PORT`. Ao alterá-la, atualize também o endereço WebSocket na interface. Este é um projeto de estudo local, sem autenticação ou histórico persistente de mensagens.

## Organização

```text
Pagina Basica de apresentação/
  index.html
  imagens/
chat de conversa/
  backend/
    package.json
    src/server.js
  frontend/
    index.html
    imagens/
```

As dependências são instaladas com `npm ci`; `node_modules/` não faz parte do repositório.

## Autor

[Yago Maba · @Yagog0](https://github.com/Yagog0)
