# 🎲 Jogo: Adivinhe o Número

Um jogo simples desenvolvido utilizando **HTML, CSS e JavaScript (Vanilla JS)**, onde o jogador deve descobrir um número aleatório entre **1 e 100**.

---

## 📸 Demonstração

### Tela Inicial

- Campo para digitar um número
- Botão **Chutar**
- Contador de tentativas

### Durante o jogo

Após cada tentativa, o sistema informa se o número secreto é:

- 📈 Maior
- 📉 Menor

### Vitória

Quando o jogador acerta:

- 🎉 Exibe uma mensagem de parabéns
- 📊 Mostra a quantidade de tentativas
- 🔄 Libera o botão **Jogar Novamente**

---

# 🚀 Tecnologias

- HTML5
- CSS3
- JavaScript (Vanilla JS)

---

# 📁 Estrutura do Projeto

```
adivinhe-numero/
│
├── index.html
├── style.css
└── script.js
```

---

# 🎮 Como Jogar

1. Abra o arquivo `index.html`.
2. Digite um número entre **1 e 100**.
3. Clique em **Chutar** ou pressione **Enter**.
4. Leia a dica apresentada.
5. Continue tentando até acertar.

---

# ⚙️ Funcionamento

Quando a página é carregada, o JavaScript cria um número aleatório:

```javascript
Math.floor(Math.random() * 100) + 1;
```

O jogador faz tentativas até encontrar esse número.

A cada tentativa:

- Soma uma tentativa
- Compara o valor digitado
- Exibe uma dica

Se:

```
chute < número secreto
```

Resultado:

```
"O número é maior."
```

Se:

```
chute > número secreto
```

Resultado:

```
"O número é menor."
```

Se acertar:

```
"Parabéns! Você acertou!"
```

---

# 🧠 Lógica do Programa

```text
Início

↓

Gerar número aleatório

↓

Usuário digita um número

↓

Número válido?

├── Não → Mostrar erro
│
└── Sim

↓

Incrementar tentativas

↓

É igual?

├── Sim
│
├── Mostrar vitória
├── Mostrar tentativas
└── Encerrar jogo
│
└── Não

↓

Número é maior?

├── Sim
│
└── Mostrar:
"O número é maior."
│
└── Não

↓

Mostrar:
"O número é menor."

↓

Esperar novo chute
```

---

# 📌 Funcionalidades

- Número aleatório de 1 a 100
- Contador de tentativas
- Mensagens de dica
- Validação de entrada
- Suporte à tecla Enter
- Botão para reiniciar a partida
- Interface responsiva

---

# 💻 Principais Conceitos Utilizados

## DOM

Manipulação dos elementos HTML.

```javascript
document.getElementById();
```

---

## Eventos

Clique no botão:

```javascript
addEventListener('click');
```

Pressionar Enter:

```javascript
addEventListener('keydown');
```

---

## Condições

```javascript
if
else
```

Para verificar:

- Acertou
- É maior
- É menor

---

## Funções

Separação da lógica em funções:

- gerarNumero()
- verificar()

---

## Variáveis

```javascript
let
const
```

Utilizadas para armazenar:

- número secreto
- tentativas
- elementos da página

---

## Números Aleatórios

```javascript
Math.random();
```

---

# 🎯 Melhorias Futuras

- Níveis de dificuldade
- Cronômetro
- Ranking de jogadores
- Sistema de pontuação
- Histórico de tentativas
- Tema escuro
- Sons e animações
- Limite de tentativas
- Estatísticas de partidas

---

# 📚 Objetivo Educacional

Este projeto foi desenvolvido para praticar os principais conceitos do JavaScript, incluindo:

- Manipulação do DOM
- Eventos
- Condições
- Funções
- Variáveis
- Números aleatórios
- Validação de entrada
- Atualização dinâmica da interface

---

# Links do projeto

[Link GitHub](https://github.com/henriquecoutinho11/senai-projeto-vanilla-js)

[Link do Deploy(vercel)](https://senai-projeto-vanilla-js.vercel.app/)

# 👨‍💻 Autor

Projeto desenvolvido como prática de **JavaScript Vanilla**, demonstrando conceitos fundamentais de programação web utilizando apenas HTML, CSS e JavaScript, sem o uso de bibliotecas ou frameworks.
