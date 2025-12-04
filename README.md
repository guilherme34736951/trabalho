Diferenças entre CSS Flexbox e CSS Grid
1. Diferenças principais
Flexbox
- Trabalha em **uma dimensão por vez** (linha **ou** coluna).
- Ideal para alinhar itens em fila, centralizações e distribuições simples.
- Os elementos são organizados com mais foco no **conteúdo**, se adaptando conforme o
espaço.
Grid
- Trabalha em **duas dimensões** (linhas **e** colunas).
- Ideal para criar **layouts completos**, estruturados e responsivos.
- Permite definir áreas, espaçamentos e alinhamentos mais complexos.
---
2. Quando Usar Cada Um
Use Flexbox quando:
- Você precisa alinhar elementos em linha ou coluna.
- O layout é simples e depende mais do fluxo natural do conteúdo.
- Exemplos:
- Menus horizontais.
- Grupos de botões.
- Cards que se rearranjam apenas em uma direção.
Use Grid quando:
- Você está criando o **layout geral da página**.
- Precisa posicionar elementos em linhas e colunas ao mesmo tempo.
- Exemplos:
- Estrutura do site: header, sidebar, main, footer.
- Galerias de imagens.
- Painéis de dashboard.
---
3. Exemplos Práticos de Projeto
Exemplo Flexbox
```css
.container {
display: flex;
justify-content: space-between;
align-items: center;
}
.card-list {
display: flex;
gap: 16px;
}
```
Exemplo Grid
```css
.layout {
display: grid;
grid-template-columns: 200px 1fr;
grid-template-rows: 80px 1fr 60px;
grid-template-areas:
"header header"
"sidebar content"
"footer footer";
}
header { grid-area: header; }
aside { grid-area: sidebar; }
main { grid-area: content; }
footer { grid-area: footer; }
```
---
Resumo Final
- **Flexbox** = controle unidimensional ® mais simples.
- **Grid** = controle bidimensional ® ideal para grandes layouts.
- Em projetos profissionais, ambos são frequentemente usados juntos.
