# ✨ A Lojinha da Lelê ✨

Site de vendas feito com muito amor para a Helena, 8 anos, vender seus produtos artesanais. 💛

## Sobre o projeto

A Lojinha da Lelê é um site estático de uma página só (`index.html`) com visual de papel de caderno e estilo desenhado à mão. A Helena cria os produtos, o papai coloca no site, e os clientes entram em contato direto pelo WhatsApp para comprar.

Sem backend, sem banco de dados, sem mensalidade. Só HTML puro com carinho.

## Funcionalidades

- Listagem de produtos organizados por categoria
- Página de detalhe de cada produto com descrição e informações de entrega
- Modal de compra que captura o nome do cliente
- Redirecionamento automático para o WhatsApp com a mensagem já formatada
- Layout responsivo, funciona bem no celular
- Visual fofo com fontes manuscritas e tema amarelo (cor favorita da Helena)

## Categorias de produtos

| Categoria | Emoji |
|---|---|
| Desenhos | 🎨 |
| Pulseiras | 💛 |
| Brinquedos Recicláveis | ♻️ |
| Ímãs de Geladeira | 🧲 |

## Como usar

### Rodar localmente

Não precisa instalar nada. Basta abrir o arquivo `index.html` direto no navegador.

```bash
# Ou rodar um servidor local simples com Python
python3 -m http.server 8080
```

### Publicar de graça

A forma mais fácil é pelo [Netlify Drop](https://app.netlify.com/drop):

1. Acesse app.netlify.com/drop
2. Arraste o arquivo `index.html` para a página
3. Pronto — você recebe um link público na hora

Também funciona no GitHub Pages, Vercel ou qualquer hospedagem de arquivos estáticos.

## Como adicionar ou editar produtos

Abra o `index.html` e localize o objeto `produtos` no JavaScript (perto do final do arquivo):

```js
const produtos = {
  "id-do-produto": {
    emoji: "🦄",
    name: "Nome do Produto",
    price: "R$ 5,00",
    desc: "Descrição do produto aqui."
  },
  // ...
};
```

Adicione uma nova entrada seguindo o mesmo padrão e crie o card correspondente no HTML, dentro da categoria correta.

## Como trocar o número do WhatsApp

No início do bloco `<script>`, troque o valor da constante `WHATSAPP`:

```js
const WHATSAPP = "5543999514569"; // DDD + número, sem espaços ou traços
```

## Tecnologias utilizadas

- HTML5 + CSS3 + JavaScript puro (sem frameworks)
- [Google Fonts](https://fonts.google.com) — fontes `Schoolbell` e `Patrick Hand`
- API do WhatsApp via link `wa.me` para contato direto

## Estrutura do projeto

```
lojinha-da-lele/
└── index.html   # o site inteiro está aqui
```

---

*Feito pela Lelê (Helena) 💛 com a ajuda do papai*
