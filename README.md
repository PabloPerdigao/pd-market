# PD MARKET | O seu e-commerce Tech

O intuito deste projeto é desenvolver uma página de promoções do PD Market colocando em prática o conhecimento sobre Git/Github, HTML5 e CSS; com foco no versionamento pelo terminal e commits bem descritos no Git, a semântica em HTML, acessibilidade e estilização.

![Vídeo do Projeto PD Market](./assets/img/preview-readme.png)


Requisitos obrigatórios:
1.  **Zero JavaScript:** Toda a interatividade (carrossel, filtros, menus) deveria ser feita apenas com CSS.
2.  **Semântica:** Uso obrigatório de uma lista de mais de 50 tags HTML5.
3.  **Git Flow:** Desenvolvimento separado por *features* em branches específicas.

---

## ✨ Funcionalidades Implementadas

### 1. Carrossel Animado (CSS-Only) 🎠
Implementação de um slider de banners com **autoplay** e **navegação manual**.
- **Técnica:** Utilizei o "Radio Button Hack".
- **Como funciona:** Inputs do tipo `radio` ocultos controlam o estado. O seletor de irmão geral (`~`) altera a margem negativa do container de slides baseada no input checado (`:checked`).
- **Sincronia:** O tempo da animação foi calculado matematicamente para permitir a reprodução completa de vídeos nos slides.

### 2. Grade de Produtos Responsiva 📱
Uma grade com mais de 30 produtos que se adapta a qualquer tamanho de tela.
- **Técnica:** CSS Grid com `repeat(auto-fill, minmax(250px, 1fr))`.
- **Detalhe:** Isso permite que os cards se reorganizem automaticamente sem a necessidade de dezenas de *media queries*.

### 3. Filtros e Sidebar Interativa 🗂️
- **Accordion:** Uso das tags nativas `<details>` e `<summary>` para criar menus que abrem e fecham sem script.
- **Sticky Sidebar:** A barra lateral acompanha a rolagem do usuário (`position: sticky`).

### 4. Semântica Rica ("Geek Mode") 🤓
Como o tema é uma loja de tecnologia, utilizei as tags obrigatórias de forma contextual:
- `<kbd>`, `<samp>`, `<var>`: Para descrições de teclados e softwares.
- `<meter>`: Para representar visualmente o **nível de estoque** dos produtos.
- `<del>` e `<strong>`: Para preços antigos e promocionais.
- `<time>`: Para datas de validade das promoções.

---

## 🛠️ Tecnologias Utilizadas

* **HTML5:** Foco total em acessibilidade e SEO (tags semânticas).
* **CSS3:**
    * Flexbox & Grid Layout.
    * Keyframe Animations (para o carrossel e pontos de navegação).
    * Pseudo-classes (`:checked`, `:hover`, `:focus`).
    * Variáveis CSS (`var(--cor-primaria)`) para consistência do tema.
* **Git/GitHub:** Controle de versão com fluxo de Feature Branch.

---

## 🌳 Estrutura do Git (Workflow)

O projeto foi desenvolvido seguindo um fluxo profissional de branches, simulando um ambiente de equipe:

1.  `main`: Código base/produção.
2.  `feature-header`: Desenvolvimento do cabeçalho, navegação e busca.
3.  `feature-carousel`: Lógica do slider CSS e banners.
4.  `feature-shop`: Catálogo de produtos, sidebar, filtros e tabelas.
5.  `feature-footer`: Rodapé, mídias, mapa e tags finais.

<br>

>  - Todas as features foram "mergeadas" na main através de Pull Requests no GitHub 
>  - Deploy do porjeto no vercel, acesse pelo link: 
https://pd-market-one.vercel.app/
