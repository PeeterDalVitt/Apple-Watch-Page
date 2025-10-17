# ⌚ Apple Watch Page

A responsive product customization page inspired by Apple's Watch storefront.  
Built entirely with **HTML, CSS, and vanilla JavaScript**, this project simulates an interactive online store experience — where users can preview different product **colors**, **sizes**, and **images** dynamically.

---

## 🖼️ Preview

<p align="center">
  <img src="./imagens/opcoes-cores/imagens-azul-inverno/imagem-1.jpeg" alt="Hashwatch screenshot" width="600">
</p>

---

## 🚀 Features

- 🎨 **Color selection:**  
  Choose between five color options (Verde-cipreste, Azul-inverno, Meia-noite, Estelar, and Rosa-claro) — all updating the main product image and title in real time.

- 🧩 **Dynamic image gallery:**  
  Clicking the thumbnails switches the main product image instantly.

- ⚙️ **Size selection:**  
  Switch between 41 mm and 45 mm, with responsive image scaling and updated titles.

- 🪶 **Clean DOM updates:**  
  Product title and color labels update dynamically through concise JavaScript logic.

- 🌱 **Carbon-neutral badge:**  
  Mimics the Apple “Carbon Neutral” label for realism.

- 💼 **Fully client-side:**  
  No frameworks or dependencies — just HTML, CSS, and vanilla JS.

---

## 🧠 Code Overview

Main logic lives in [`script.js`](./script.js):

- **`atualizarCorSelecionada()`** → Handles color selection and updates all images + product title.  
- **`atualizarTamanho()`** → Adjusts product details and image scale based on selected size.  
- **`atualizarImagemSelecionada()`** → Changes the main image to match the selected thumbnail.  

All state is managed through simple index variables:
```js
let numImagemSelecionada = 1;
let numTamanhoSelecionado = 1;
let numCorSelecionada = 1;
