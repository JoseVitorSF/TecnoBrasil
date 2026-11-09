# 🛒 TecnoBrasil

> **Tecnologia com o DNA brasileiro**

Loja virtual de eletrônicos e periféricos gamer, desenvolvida com HTML, CSS e JavaScript puro. O projeto conta com vitrine de produtos em promoção, carrinho de compras dinâmico, pagamento via PIX (simulado) e telas de login e cadastro.

![Logo TecnoBrasil](Ingoude.jpg)

---

## 📋 Índice

- [Funcionalidades](#-funcionalidades)
- [Tecnologias](#-tecnologias)
- [Estrutura do projeto](#-estrutura-do-projeto)
- [Como executar](#-como-executar)
- [Como funciona o carrinho](#-como-funciona-o-carrinho)
- [Produtos](#-produtos)
- [Pendências e melhorias](#-pendências-e-melhorias)
- [Autor](#-autor)

---

## ✨ Funcionalidades

- 🏠 **Página inicial** com banner, menu de navegação e seção de produtos em promoção
- 🛍️ **Carrinho de compras** que atualiza itens e total em tempo real
- 💸 **Pagamento via PIX** (simulado, com alerta de confirmação)
- 🔐 **Tela de login** (e-mail e senha)
- 📝 **Tela de cadastro** (nome completo, e-mail e senha)
- 🪟 **Exemplo de modal** com imagem para exibir o pagamento (QR Code PIX)
- 🎨 **Visual personalizado** em tons de roxo e preto, com efeito de zoom nos produtos

---

## 🧰 Tecnologias

| Tecnologia | Uso |
|---|---|
| HTML5 | Estrutura das páginas |
| CSS3 | Estilização (Flexbox, transições, sombras) |
| JavaScript (ES6) | Lógica do carrinho e do modal |
| PHP *(previsto)* | Processamento de login e cadastro |

---

## 📁 Estrutura do projeto

```
tecnobrasil/
├── index.html          # Página inicial (produtos + carrinho)
├── produtos.html       # Página de produtos
├── login.html          # Tela de login
├── cadastro.html       # Tela de cadastro
├── new 1.html.txt      # Exemplo de modal de pagamento
├── style.css           # Estilos do site
├── login.css           # Estilos de login e cadastro
├── Ingoude.jpg         # Logo / banner da loja
└── qr-code-plus.jpg    # QR Code da loja
```

---

## 🚀 Como executar

Não é necessário instalar nada para visualizar o front-end.

1. **Baixe ou clone** o projeto:
   ```bash
   git clone https://github.com/seu-usuario/tecnobrasil.git
   ```
2. **Abra a pasta** do projeto.
3. **Dê dois cliques** em `index.html` para abrir no navegador.

> 💡 Para testar `login.php` e `cadastro.php`, será necessário um servidor com PHP (como XAMPP, WAMP ou `php -S localhost:8000`).

---

## 🛒 Como funciona o carrinho

1. O cliente clica em **Comprar** em um produto.
2. O item é adicionado à lista do **Carrinho de Compras**.
3. O **total** é recalculado automaticamente.
4. Ao clicar em **Pagar com PIX**, o sistema:
   - confirma o pagamento com o valor total;
   - limpa o carrinho;
   - exibe um aviso caso o carrinho esteja vazio.

---

## 🖥️ Produtos

| Produto | Preço |
|---|---|
| Teclado Gamer Logitech G | R$ 749,00 |
| Notebook Gamer Acer Nitro | R$ 4.999,00 |
| Placa de Vídeo GeForce GTX 1650 4GB | R$ 849,00 |
| Headset Gamer HyperX Cloud Alpha | R$ 449,00 |

---

## 🔧 Pendências e melhorias

Itens identificados na revisão do código para as próximas versões:

- [ ] Preencher o `login.css` (está vazio, então login e cadastro ficam sem estilo)
- [ ] Criar o conteúdo da página `produtos.html` (está vazia)
- [ ] Criar os arquivos `login.php` e `cadastro.php` referenciados nos formulários
- [ ] Corrigir as imagens do array `produtos` no JavaScript (usam links `example.com`, que não existem; o array não é exibido na tela, mas vale ajustar)
- [ ] Associar cada botão **Comprar** ao produto por `data-id`, em vez de depender da ordem dos botões
- [ ] Integrar o modal de pagamento (`new 1.html.txt`) com o QR Code PIX real ao finalizar a compra
- [ ] Salvar o carrinho com `localStorage` para não perder os itens ao recarregar
- [ ] Tornar o layout responsivo para celular
- [ ] Hospedar as imagens dos produtos localmente (evita links quebrados)
- [ ] Armazenar senhas com hash (`password_hash`) no back-end

---

## 👤 Autor

Desenvolvido por **[Seu Nome]**.

📧 contato: seu-email@exemplo.com

---

<p align="center">© 2024 TecnoBrasil — Tecnologia com o DNA brasileiro 🇧🇷</p>
