
## ☕ CAFENA - Café da Região: Projeto MVP

Este é um *Minimum Viable Product* **(MVP)** desenvolvido para a **CAFENA**, uma cafeteria fictícia focada em promover o **café da região**. O projeto tem como objetivo principal apresentar a marca, o menu e a localização de forma clara e totalmente **responsiva**, garantindo uma boa experiência tanto em desktops quanto em dispositivos móveis.

-----

### ✨ Funcionalidades Principais do MVP

O projeto foi construído utilizando **HTML** e **CSS** puros (sem *frameworks*), focando nas seguintes seções:

- **Home (Hero):** Apresentação visual de impacto com uma chamada de ação ("Pegue o seu Agora").

- **Sobre Nós:** Detalhes sobre o que torna o café da CAFENA especial, com layout flexível que se adapta à tela.

- **Menu:** Exibição dos itens principais do menu (Expresso, Cappuccino, Mocha, etc.).

- **Avaliações (Review):** Seção para construir prova social, mostrando depoimentos de clientes.

- **Endereço:** Localização da cafeteria através de um *iframe* do mapa.
---
### 💻 Responsividade e Interatividade (Destaques Técnicos)
O foco do desenvolvimento foi em criar um design que funciona perfeitamente em qualquer tamanho de tela.

#### 1. Menu Sanduíche (Mobile-First)
- O menu principal é transformado em um **menu sanduíche** (`.menu-btn`) **em telas com largura menor ou igual a 767px**.

- A navegação e os ícones de busca/carrinho (`.icons`) são ocultados no mobile para otimizar o espaço do cabeçalho.

- A lógica de abertura e fechamento do menu sanduíche utiliza o **"Checkbox Hack"** (seletores `:checked` e `~`), dispensando a necessidade de JavaScript.

  - Quando o ícone (`<label class="menu-btn">`) é clicado, o estado do `<input type="checkbox" id="menu-toggle">` muda, acionando a animação de deslize do menu (`<nav>`) através da propriedade `clip-path`.

#### 2. Estilos Adaptáveis (Media Queries)
Foram utilizadas *media queries* para adaptar o layout e as fontes, garantindo a legibilidade e o espaçamento adequado:

##### 📐 Tabela de Responsividade e Quebra de Layout

| Elemento | Tamanho Base (Desktop) | Tamanho Mobile (`max-width: 767px`) |
| :--- | :--- | :--- |
| **Título Principal (Home)** | `6rem` | Reduzido para `4.5rem` |
| **Títulos de Seção** | `4rem` | Reduzido para `3rem` |
| **Layouts** | Grid de 3 colunas (`.box-container`) | Grid de 1 coluna (`1fr`) |

### 🚀 Como Executar o Projeto
1. Baixe ou clone os arquivos `index.html` e `style.css`.

2. Abra o arquivo `index.html` em qualquer navegador.

3. Redimensione a janela do navegador (ou use as ferramentas de desenvolvedor) para visualizar a responsividade do menu sanduíche.
