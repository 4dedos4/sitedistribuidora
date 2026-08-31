# JS Distribuidora de Água e Gás — Site

Site institucional estático (HTML/CSS/JS puro, sem build) para a JS Distribuidora de Água e Gás, focado em direcionar clientes para o WhatsApp e apresentar o catálogo de produtos (água, gás, carvão, refrigerante e cerveja).

## Estrutura

```
index.html      Página única com todas as seções
css/style.css   Estilos (tema vermelho/preto, responsivo mobile-first)
js/script.js    Menu mobile e rodapé dinâmico
```

## Como rodar localmente

Abra `index.html` direto no navegador, ou sirva a pasta com qualquer servidor estático, por exemplo:

```bash
python3 -m http.server 8000
```

## Personalização

- **WhatsApp**: os links usam `https://wa.me/55...` com os números (98) 98451-1449 e (98) 99952-7295. Troque o número e a mensagem pré-preenchida direto nos atributos `href` do `index.html`.
- **Logo**: atualmente é um badge "JS" em CSS (`.logo-badge`). Para usar a logo real, adicione o arquivo de imagem em uma pasta `img/` e troque o `<span class="logo-badge">JS</span>` por uma tag `<img>`.
- **Endereço/mapa**: o mapa embutido usa o endereço "Av. Amizael Gomes da Silva, 5327" via Google Maps embed público (sem necessidade de API key).
- **Produtos**: cada card em `#produtos` já tem um link de WhatsApp com mensagem pré-preenchida específica do produto.

## Publicar (GitHub Pages)

1. Nas configurações do repositório, ative GitHub Pages apontando para a branch desejada e pasta raiz (`/`).
2. O site ficará disponível em `https://<usuario>.github.io/<repositorio>/`.
