# Frameworks CSS

## Frameworks Front-end

**Prof. Me. Deivison S. Takatu**

deivison.takatu@edu.senai.br

---

# Sumário

- API (Application Programming Interface)
- Protocolo HTTP
- EndPoint
- JSON (JavaScript Object Notation)
- Atividade 01
- Servidor Backend e Web Service
- Criando uma API REST com Express
- Atividade 02

---

# Cascading Style Sheets

O CSS não só define cores e fontes, como também controla margens, alinhamentos, larguras, alturas e elementos flutuantes, garantindo páginas organizadas e responsivas.

Com suas propriedades, é possível alinhar componentes, distribuir espaços e criar layouts elegantes que unem estética e funcionalidade.

---

# Estrutura do CSS

O CSS segue a estrutura:

```css
seletor {
    propriedade: valor;
}
```

- O seletor indica em qual tag HTML a regra será aplicada.
- A propriedade define o atributo a ser modificado, como a cor de fundo (`background-color`).
- O valor especifica a configuração desejada, como `#FF0000` para vermelho.
- Essa combinação permite personalizar a aparência de páginas web.

---

# CSS e HTML

Muitas propriedades do CSS são semelhantes às usadas no HTML, mas oferecem maior flexibilidade e padronização.

Por exemplo, para definir um fundo vermelho em uma página:

### HTML

```html
<body bgcolor="#FF0000">
```

### CSS

```css
body {
    background-color: #FF0000;
}
```

---

# Aplicação do CSS

Existem três formas principais de aplicar CSS:

## CSS In-line

Aplicado diretamente no elemento HTML, usando o atributo `style`. Indicado apenas para testes ou ajustes pontuais.

## CSS Interno

Definido dentro da tag `<style>` no cabeçalho da página. Útil quando o estilo será usado apenas em uma única página.

## CSS Externo

Escrito em um arquivo separado `.css` e vinculado ao HTML com a tag `<link>`. É a forma mais recomendada, pois organiza e reutiliza o estilo em várias páginas.

---

# Aplicação do CSS - In Line

O estilo in-line é aplicado diretamente em um elemento HTML utilizando o atributo `style`. Essa abordagem permite alterar rapidamente a aparência de um único componente, sem a necessidade de criar regras adicionais em arquivos separados.

### Exemplo

```html
<p style="color: red; font-size: 20px;">Este é um texto em vermelho e maior</p>
```

---

# Aplicação do CSS - Interno

O estilo interno é definido dentro da tag `<style>` do documento HTML. É ideal quando queremos aplicar estilos apenas a uma única página ou testar rapidamente mudanças visuais sem alterar outros arquivos.

### Exemplo

```html
<style>
    p { color: blue; font-size: 18px; }
</style>
```

---

# Aplicação do CSS - Externo

O estilo externo é definido em um arquivo separado com extensão `.css` e vinculado ao documento HTML através da tag `<link>`. Essa abordagem é a mais recomendada para projetos maiores, pois permite centralizar todos os estilos em um único arquivo, facilitando a manutenção e a consistência visual em várias páginas do site.

### Exemplo

```html
<link rel="stylesheet" href="estilos.css">
```

---

# Propriedades do CSS

## Color

Define a cor do texto dentro de um elemento.

```css
color: #ff0000;
```

ou

```css
color: red;
```

## Background-color

Define a cor de fundo de um elemento.

```css
background-color: #0000ff;
```

ou

```css
background-color: blue;
```

## Font-family

Especifica a fonte a ser usada para o texto.

```css
font-family: Arial, sans-serif;
```

---

# Propriedades do CSS

## Font-size

Controla o tamanho do texto. Pode ser definido em pixels, ems, rems, porcentagem, etc.

```css
font-size: 16px;
```

ou

```css
font-size: 1.2rem;
```

## Margin

Controla o espaço fora das bordas de um elemento, criando distância entre ele e outros elementos.

```css
margin: 20px;
```

Margem uniforme.

```css
margin: 10px 5px 15px 20px;
```

Ordem:

```text
top
right
bottom
left
```

## Padding

Controla o espaço dentro das bordas de um elemento, entre a borda e seu conteúdo.

```css
padding: 15px;
```

Padding uniforme.

```css
padding: 10px 20px;
```

Ordem:

```text
vertical
horizontal
```

---

# Propriedades do CSS

## Border

Define a espessura, o estilo e a cor da borda ao redor de um elemento.

```css
border: 2px solid black;
```

## Width e Height

Controlam as dimensões de um elemento.

```css
width: 300px;
height: 200px;
```

## Display

Define como um elemento é renderizado na página.

```css
display: block;
```

```css
display: inline;
```

```css
display: flex;
```

---

# Propriedades do CSS

## Position

Especifica o método de posicionamento de um elemento: estático, relativo, absoluto ou fixo.

```css
position: relative;
```

```css
position: absolute;
```

```css
position: fixed;
```

## Top, Right, Bottom, Left

Usadas junto com a propriedade `position` para posicionar um elemento de forma precisa.

```css
top: 10px;
left: 20px;
```

## Text-align

Controla o alinhamento horizontal do texto dentro de seu elemento container.

```css
text-align: center;
```

```css
text-align: justify;
```

---

# Class e ID

## Classes

Classes permitem aplicar o mesmo estilo a múltiplos elementos, garantindo consistência visual e facilitando a manutenção do código.

### Exemplo

```css
.botao-primario {
    background: blue;
    color: red;
    padding: 10px;
}
```

## IDs

IDs são utilizados para estilizar elementos únicos e específicos da página, além de permitirem a navegação via âncora e a manipulação via JavaScript de forma precisa.

### Exemplo

```css
#cabecalho-principal {
    height: 80px;
    background: #333;
}
```

---

# Atividade de Revisão

Link: https://wayground.com/

Material: https://github.com/deivisontakatu/aula-css

---

# Box Model

O box model (modelo das caixas) em CSS descreve os boxes gerados pelos elementos HTML. O box model detalha ainda, as opções de ajuste de margens, bordas, padding e conteúdo para cada elemento.

---

# Box Model - Por que aplicar?

- Controlar o tamanho dos elementos;
- Criar espaçamento e organização visual;
- Evitar sobreposição e problemas de dimensionamento;
- Construir layouts mais previsíveis;
- Facilitar a adaptação dos elementos para diferentes telas.

---

# Box Model - Elementos

- **Content:** Área onde o texto e imagens aparecem.
- **Padding:** Espaço entre o conteúdo e a borda.
- **Border:** Linha que envolve o padding e conteúdo.
- **Margin:** Espaço entre a borda e outros elementos.

---

# FlexBox

O Flexbox (Flexible Box Layout) é um módulo de layout unidimensional projetado para organizar itens em linhas ou colunas, oferecendo distribuição de espaço e alinhamento.

---

# FlexBox - Propriedades

- `flex-direction: row | column`
- `justify-content: flex-start, center, space-between, space-around`
- `align-items: flex-start, center, flex-end`
- `flex-wrap`: permite quebra de linha
- `gap`: define espaçamento entre itens

---

# FlexBox - Materiais visuais

A aula apresenta materiais visuais sobre FlexBox com as seguintes fontes:

- freecodecamp.org
- dio.me

---

# Layouts Responsivos

- Técnica de design que adapta o conteúdo para diferentes tamanhos de tela (celular, tablet, desktop).
- Melhora a usabilidade e a experiência do usuário.
- Reduz a necessidade de criar versões separadas para cada dispositivo.

---

# Atividade 01

1. Crie um projeto e utilize os arquivos `index.html` e `style.css`, incluindo o CSS de forma Externa ao HTML, através da tag `<link>`.

2. Adicione 20 elementos e atribua valores em todas as propriedades de Content, Padding, Border e Margin.

3. Em seguida, adicione 20 propriedades de Flexbox para manipular os elementos e organizá-los de forma responsiva.

---

# O que é um Framework CSS?

Um framework CSS é um conjunto de recursos, padrões, classes e componentes que facilita a criação e a padronização de interfaces web.

---

# Componentes Framework CSS

## Layout

- Grid
- Flexbox
- responsividade

## Estilos

- Cores
- espaços
- tipografia

## Componentes

- Botões
- cards
- navbar

---

# O Problema do CSS Manual

## Exemplo prático

```html
<button class="botao">
    Enviar
</button>
```

```css
.botao {
    background: #2563eb;
    color: white;
    padding: 12px 24px;
    border-radius: 8px;
}
```

Tudo precisa ser estilizado:

- Botões e cards
- Formulários e menus
- Grid e responsividade
- Espaçamentos e tipografia

---

# Tailwind CSS

Tailwind CSS é um framework CSS baseado principalmente no conceito Utility-First.

Em vez de fornecer apenas componentes prontos, o Tailwind fornece pequenas classes que representam propriedades de estilo.

Utility-First é uma abordagem de desenvolvimento em que pequenas classes CSS possuem uma responsabilidade específica e podem ser combinadas para construir uma interface.

---

# Propósitos do Tailwind CSS

- **Reduzir o tempo de desenvolvimento:** Utilizar classes utilitárias para estilização diretamente no HTML.
- **Aumentar a flexibilidade da interface:** Permitir a composição de componentes sem depender de estilos predefinidos.
- **Facilitar a customização:** Centralizar e adaptar facilmente cores, espaçamentos, tipografia e demais propriedades.
- **Promover reutilização e consistência:** Utilizar um sistema padronizado de classes e tokens de design.
- **Simplificar o desenvolvimento responsivo:** Aplicar uma abordagem Mobile First de forma integrada ao framework.

---

# Tailwind CSS - Exemplo Utility-First

```text
p-6
```

→ define padding

```text
text-xl
```

→ define tamanho do texto

```text
font-bold
```

→ define peso da fonte

```text
bg-blue-600
```

→ define cor de fundo

```text
rounded-lg
```

→ define bordas arredondadas

Para um card, criamos:

```text
p-6 bg-white rounded-xl shadow
```

**IDEIA:**

> Uma utility = uma responsabilidade.

> Várias utilities = um componente.

---

# Tailwind CSS

O Tailwind permite construir componentes combinando pequenas classes utilitárias diretamente no HTML, sem criar classes CSS separadas.

## Classes do exemplo

```text
bg-blue-600
```

Cor de fundo.

```text
text-white
```

Cor do texto.

```text
px-6 py-3
```

Padding horizontal e vertical.

```text
rounded-lg
```

Bordas arredondadas.

### Código

```html
<button class="bg-blue-600 text-white px-6 py-3 rounded-lg">
    Enviar
</button>
```

---

# Importando Tailwind CSS - Play CDN

Ideal para testes.

No `index.html`, dentro do `<head>`:

```html
<script src="https://cdn.jsdelivr.net/npm/@tailwindcss/browser@4">
</script>
```

Documentação:

https://tailwindcss.com/docs

---

# Importando Tailwind CSS - Tailwind CLI

## Passo 1: Instalar Tailwind CLI

```bash
npm install tailwindcss @tailwindcss/cli
```

## Passo 2: Importar no CSS

```css
@import "tailwindcss";
```

## Passo 3: Integração do Tailwind ao processo de transformação do CSS

```bash
npm install tailwindcss @tailwindcss/postcss postcss
```

## Passo 4: Integração com frameworks

O Tailwind possui procedimentos específicos de instalação para diferentes frameworks e ferramentas.

---

# Tailwind CSS - Integração com frameworks

O Tailwind CSS pode ser integrado a diferentes frameworks e ferramentas de desenvolvimento, seguindo as configurações específicas de cada ambiente.

Essa integração permite incorporar o Tailwind ao processo de desenvolvimento, compilação e geração dos arquivos da aplicação.

Frameworks como Next.js, Laravel, Angular e Ruby on Rails possuem orientações próprias para instalação e configuração.

O objetivo é adaptar o Tailwind à estrutura utilizada pelo projeto, mantendo o processo de desenvolvimento integrado às ferramentas já existentes.

---

# Instalação do Tailwind IntelliSense

- **Extensão para editores de código:** Oferece suporte ao desenvolvimento com Tailwind CSS.
- **Autocompletar classes:** Sugere automaticamente classes e propriedades disponíveis no framework.
- **Visualização de estilos:** Apresenta informações sobre as classes utilizadas durante a codificação.
- **Apoio ao desenvolvimento:** Reduz erros de digitação e facilita a utilização das classes utilitárias.

---

# Tailwind CSS Classes

- Classes são identificadores utilizados para aplicar estilos a elementos HTML.
- No Tailwind CSS, cada classe representa uma regra ou conjunto específico de estilos.
- As classes são combinadas diretamente no atributo `class` do elemento.
- Essa abordagem permite construir a interface utilizando classes utilitárias, sem precisar criar uma regra CSS para cada componente.

Fonte: https://tailwind.build/classes

---

# Atividade 02

1. Crie um projeto que utilize pelo menos 30 classes diferentes do Tailwind CSS. As classes devem ser utilizadas para definir elementos como cores, tipografia, espaçamentos, dimensões, bordas, posicionamento, flexbox, grid e responsividade.

2. Organize a entrega em um repositório, e documente através de um markdown, contendo:
   - prints do código;
   - da aplicação em funcionamento;
   - uma lista das classes utilizadas com suas respectivas funções;
   - o link para o projeto desenvolvido.

---

# Referências

1. SOUZA, Natan. **Bootstrap 4: conheça a biblioteca front-end mais utilizada no mundo.** São Paulo: Casa do Código, 2018. E-book. Disponível em: https://plataforma.bvirtual.com.br.

2. MACHADO, Kheronn Khennedy. **Angular 11 e Firebase: construindo uma aplicação integrada com a plataforma do Google.** São Paulo: Casa do Código, 2021. E-book. Disponível em: https://plataforma.bvirtual.com.br. Acesso em: 13 maio 2025.

3. EIS, Diego. **Guia Front-end: o caminho das pedras para ser um dev front-end.** São Paulo: Casa do Código, 2015. E-book. Disponível em: https://plataforma.bvirtual.com.br.

4. GONÇALVES, Edson. **Desenvolvendo aplicações Web com JSP, Servlets, JavaServer Faces, Hibernate, EJB 3 Persistence e Ajax.** Rio de Janeiro: Ciência Moderna, c2007.

5. HARTCOPP, Patrícia Ferreira. **Métrica Web.** São Paulo: Contentus, 2020. E-book (94 p.). Disponível em: https://plataforma.bvirtual.com.br/Acervo/Publicacao/185191. Acesso em: 30 abr. 2024.

6. NIEDERAUER, Juliano. **Desenvolvendo Websites com PHP: aprenda a criar Websites dinâmicos e interativos com PHP e banco de dados.** 3. ed. São Paulo: Novatec, 2017.

7. PREECE, J.; ROGERS, Y.; SHARP, H. **Design de Interação: além da interação Homem-Computador.** 3. ed. Porto Alegre: Bookman, 2013.

8. SOUSA, Roque Fernando Marcos. **Canvas HTML 5: composição gráfica e interatividade na Web.** Rio de Janeiro: Brasport, 2014. E-book (194 p.). Disponível em: https://plataforma.bvirtual.com.br/Acervo/Publicacao/160686. Acesso em: 22 jun. 2024.

---

# Frameworks CSS

## Frameworks Front-end

**Prof. Me. Deivison S. Takatu**

deivison.takatu@edu.senai.br
