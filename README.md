# 🎨 CSS COMPLETO —

> 📚 Guia EXTREMAMENTE COMPLETO de CSS para Fullstack Iniciante.

---

# 📍 INTRODUÇÃO AO CSS

## 🎯 O que é CSS?

CSS significa:

```css
Cascading Style Sheets
```

Responsável pela aparência do site.

---

## 🧠 O que CSS faz?

- altera cores
- muda fontes
- cria layouts
- cria responsividade
- cria animações

---

## 🌎 Relação HTML + CSS

```css
HTML → estrutura
CSS → aparência
JavaScript → interatividade
```

---

# 📍 SINTAXE CSS

## 🧱 Estrutura básica

```css
h1 {
  color: red;
}
```

---

## 🔍 Explicação

| Parte | Função      |
| ----- | ----------- |
| h1    | seletor     |
| color | propriedade |
| red   | valor       |

---

# 📍 COMO ADICIONAR CSS

---

## 🔹 1. Inline

O CSS é colocado diretamente dentro da tag HTML usando `style`.

### ✅ Exemplo

```html
<h1 style="color:red;">Título vermelho</h1>
```

### 🧠 Como funciona

- `style=""` recebe propriedades CSS.
- `color:red` muda a cor do texto.

### ✅ Vantagem

- rápido para testes

### ❌ Desvantagem

- difícil manutenção
- código fica bagunçado

---

## 🔹 2. CSS Interno

O CSS fica dentro da própria página HTML usando `<style>`.

### ✅ Exemplo

```html
<style>
  h1 {
    color: red;
  }
</style>
```

### 🧠 Explicação

- `h1` → seletor
- `{}` → bloco de regras
- `color:red` → propriedade + valor

Todos os `<h1>` ficarão vermelhos.

---

## 🔹 3. CSS Externo (mais usado)

O CSS fica separado em um arquivo `.css`.

### ✅ HTML

```html
<link rel="stylesheet" href="style.css" />
```

### ✅ style.css

```css
h1 {
  color: red;
}
```

### 🧠 Vantagens

- organização profissional
- reutilização
- manutenção fácil
- melhor performance

---

# 📍 SELETORES

Seletores dizem QUAL elemento será estilizado.

---

## 🔹 Elemento

Seleciona pela tag.

```css
p {
  color: blue;
}
```

Todos os `<p>` ficam azuis.

---

## 🔹 Classe

Usa `.`

### HTML

```html
<div class="card"></div>
```

### CSS

```css
.card {
  background: gray;
}
```

### 🧠 Classe é reutilizável

Pode usar em vários elementos.

---

## 🔹 ID

Usa `#`

### HTML

```html
<h1 id="titulo"></h1>
```

### CSS

```css
#titulo {
  font-size: 40px;
}
```

### 🧠 ID deve ser único.

---

## 🔹 Universal

Seleciona TODOS elementos.

```css
* {
  margin: 0;
}
```

Muito usado para resetar estilos.

---

## 🔹 Descendente

Seleciona elementos dentro de outros.

```css
div p {
  color: red;
}
```

Todos os `<p>` dentro de `div`.

---

## 🔹 Filho direto

```css
div > p {
  color: blue;
}
```

Somente filhos diretos.

---

# 📍 CORES

---

## 🎨 Color

Muda cor do texto.

```css
color: red;
```

---

## 🎨 RGB

```css
color: rgb(255, 0, 0);
```

RGB:

- Red
- Green
- Blue

Vai de 0 até 255.

---

## 🎨 HEX

```css
color: #ff0000;
```

Formato hexadecimal.

Muito usado profissionalmente.

---

## 🎨 HSL

```css
color: hsl(0, 100%, 50%);
```

HSL:

- Hue
- Saturation
- Lightness

---

## 🌈 Background

Cor de fundo.

```css
background-color: black;
```

---

## 🖼️ Imagem de fundo

```css
background-image: url('img.jpg');
```

---

# 📍 FONTES E TEXTOS

---

## 🔠 Font-size

Tamanho do texto.

```css
font-size: 20px;
```

---

## 🔡 Font-family

Fonte.

```css
font-family: Arial;
```

---

## 🔥 Font-weight

Peso da fonte.

```css
font-weight: bold;
```

---

## ✨ Italic

```css
font-style: italic;
```

---

## 📏 Line-height

Espaço entre linhas.

```css
line-height: 1.5;
```

---

## 🔤 Text-align

Alinhamento.

```css
text-align: center;
```

---

## 🔠 Text-transform

Transforma texto.

```css
text-transform: uppercase;
```

---

# 📍 ESPAÇAMENTOS

---

## 📦 Margin

Espaço EXTERNO.

```css
margin: 20px;
```

---

## 📦 Padding

Espaço INTERNO.

```css
padding: 20px;
```

---

## 📏 Width

Largura.

```css
width: 300px;
```

---

## 📏 Height

Altura.

```css
height: 200px;
```

---

# 📍 BOX MODEL

Todo elemento HTML é uma caixa.

Estrutura:

```txt
Margin
Border
Padding
Content
```

---

## 🔲 Border

Borda.

```css
border: 2px solid black;
```

---

## 🔘 Border-radius

Arredondamento.

```css
border-radius: 10px;
```

---

## 🌫️ Shadow

Sombra.

```css
box-shadow: 0 0 10px black;
```

---

# 📍 DISPLAY

Controla comportamento do elemento.

---

## 🔹 Block

Ocupa linha inteira.

```css
display: block;
```

---

## 🔹 Inline

Fica na mesma linha.

```css
display: inline;
```

---

## 🔹 Inline-block

Mistura dos dois.

```css
display: inline-block;
```

---

## 🔹 None

Esconde elemento.

```css
display: none;
```

---

## 🔥 Flex

Layout flexível.

```css
display: flex;
```

---

## 🔥 Grid

Layout em grade.

```css
display: grid;
```

---

# 📍 POSITION

---

## 🔹 Relative

Base para posicionamento.

```css
position: relative;
```

---

## 🔹 Absolute

Posiciona livremente.

```css
position: absolute;
```

---

## 🔹 Fixed

Fica preso na tela.

```css
position: fixed;
```

---

## 🔹 Sticky

Gruda ao rolar.

```css
position: sticky;
```

---

# 📍 FLEXBOX

Usado para alinhamento.

---

## 🎯 Container

```css
.container {
  display: flex;
}
```

---

## 🔹 Direção

```css
flex-direction: row;
flex-direction: column;
```

---

## 🔹 Horizontal

```css
justify-content: center;
```

---

## 🔹 Vertical

```css
align-items: center;
```

---

## 🔹 Espaçamento

```css
gap: 20px;
```

---

## 🔥 Centralização perfeita

```css
display: flex;
justify-content: center;
align-items: center;
height: 100vh;
```

---

# 📍 GRID

Sistema de colunas e linhas.

---

## 🔹 Colunas

```css
grid-template-columns: 1fr 1fr 1fr;
```

---

## 🔹 Linhas

```css
grid-template-rows: 100px 100px;
```

---

# 📍 RESPONSIVIDADE

Adaptar para celulares.

---

## 📱 %

```css
width: 100%;
```

---

## 📱 Viewport

```css
width: 100vw;
height: 100vh;
```

---

## 📱 REM

Escala responsiva.

```css
font-size: 1rem;
```

---

# 📍 MEDIA QUERIES

Mudam CSS conforme tamanho da tela.

---

## 📱 Mobile

```css
@media (max-width: 768px) {
}
```

---

## 💻 Desktop

```css
@media (min-width: 1024px) {
}
```

---

# 📍 PSEUDO-CLASSES

Mudam comportamento.

---

## ✨ Hover

Quando passa mouse.

```css
button:hover {
  background: red;
}
```

---

## ✨ Focus

Quando seleciona input.

```css
input:focus {
  border: 2px solid blue;
}
```

---

# 📍 PSEUDO-ELEMENTOS

Criam elementos virtuais.

---

## 🔥 Before

```css
p::before {
  content: '🔥';
}
```

---

## 🔥 After

```css
p::after {
  content: '🚀';
}
```

---

# 📍 TRANSITIONS

Anima suavemente.

```css
transition: 0.3s;
```

---

# 📍 ANIMAÇÕES

---

## 🎬 Keyframes

```css
@keyframes slide {
  from {
    opacity: 0;
  }

  to {
    opacity: 1;
  }
}
```

---

## 🎯 Aplicação

```css
animation: slide 2s infinite;
```

---

# 📍 TRANSFORM

---

## 🔹 Scale

Aumenta.

```css
transform: scale(1.2);
```

---

## 🔹 Rotate

Gira.

```css
transform: rotate(45deg);
```

---

## 🔹 Translate

Move.

```css
transform: translateX(50px);
```

---

# 📍 VARIÁVEIS CSS

---

## 🎨 Root

```css
:root {
  --primary: #ff0000;
}
```

---

## 🔥 Uso

```css
color: var(--primary);
```

---

# 📍 ORGANIZAÇÃO PROFISSIONAL

```txt
css/
 ├── style.css
 ├── variables.css
 ├── reset.css
 ├── layout.css
 └── components.css
```

---

# 📘 DICAS IMPORTANTES

✅ Use classes ao invés de IDs

✅ Prefira CSS externo

✅ Organize por componentes

✅ Use Flexbox e Grid

✅ Faça layouts responsivos

✅ Nomeie classes claramente

### Exemplo

```css
.navbar
.card-produto
.botao-login
```
