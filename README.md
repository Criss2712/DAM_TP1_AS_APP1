# Assignment 1 — Hello Android World!
<!-- Replace X and Title -->
Course: Desenvolvimento de Aplicações Móveis (DAM)

Student(s): Renata Cristina Conceição Góis

Date: 10/03/2026

Repository URL: https://github.com/Criss2712/DAM_TP1_AS_APP1

---

## 1. Introduction
<!-- Purpose of the assignment, problem description, and objectives. -->

No seguimento do primeiro trabalho prático, o presente repositório destina-se a apresentar à primeira
aplicação Android desenvolvida no IDE Android Studio. A aplicação HelloWorldV2 foi desenvolvida como
um exercício introdutório ao desenvolvimento Android, com o objetivo de explorar conceitos 
fundamentais como layouts, personalização de temas, adaptação a diferentes orientações de ecrã.
Começou-se por um genérico "Hello World!", e terminou-se numa aplicação com um bocado de mais personalização.

## 2. System Overview
<!-- High-level description of the solution, main features, and use cases. -->

A aplicação desenvolvida apresenta um ecrã princinpal composto por:

- Uma toolbar personalizada com o título "Hello World V2";
- Duas componentes `TextViews` com estilos personalizados;
- Uma imagem e um calendário interativo.

## 3. Architecture and Design
<!-- Architecture, folder structure, design patterns, and justification of key
    decisions. -->

A aplicação segue a aquiterura já pré-definida de uma aplicação Android:

- `MainActivity.kt`: Ficheiro Kotlin com a lógica principal da aplicação

- `res\`:
  - `layout\acticity_main\activity_main.xml`: Ficheiro responsável pelo Layout Portrait
  
  - `layout\activity_main.xml(land)`: Ficheiro responsável pelo Layout Landscape
  - `values\strings.xml`: Ficheiro que contém as strings internaciolizadas
  - `values\colors.xml` Ficheiro que contém as cores internaciolizadas
  - `values\themes.xml` Ficheiro que contém a personalização do tema da aplicação
  - `drawable`: Pasta que contém as imagens utilizadas

**Decisões de design:**
- **Toolbar personalizada:** Em vez da ActionBar padrão, para maior controlo visual
- **Ficheiros de layout separados:** Para portrait e landscape, garantindo melhor experiência em cada orientação
- **Cores personalizadas:** Definidas em colors.xml para consistência e fácil manutenção
    
## 4. Implementation
<!-- Implementation details: main modules, components, algorithms, and relevant code
    excerpts. -->

A primeira versão da aplicação, **"Hello World V1"**, consistiu apenas na apresentação de "Hello World" 
e na internalização da string correspondente ao texto apresentado, no ficheiro `strings.xml`.

Na segunda versão adicionaram-se mais componentes, como mais componentes de texto personalizadas com
cores, previamente definidas em `colors.xml`, uma imagem e um calendário. Personalizou-se também a 
toolBar para uma cor diferente da pré-definida pelo tema utizado:

```xml
<resources xmlns:tools="http://schemas.android.com/tools">
    <!-- Base application theme. -->
    <style name="Base.Theme.HelloWorld" parent="Theme.AppCompat.Light.DarkActionBar">
    </style>

    <style name="Theme.HelloWorld" parent="Base.Theme.HelloWorld">
        <item name="colorPrimary">@color/rich_cerulean</item>
    </style>
</resources>
```

Após essas adições, adicionou-se também um ícone da aplicação, e um modo landscape da mesma.


## 5. Testing and Validation
<!-- Testing strategy, test cases, scenarios, edge cases, and known limitations. -->

Foram realizados testes às posições das componentes no ecrã de modo a não ficarem escondidas atrás da
toolBar. À correta utilização das cores escolhidas, e às duas versões de apresentação, portrait e 
landscape para verificar se transicionavam entre os dois. 


## 6. Usage Instructions
<!-- How to run the project: requirements, setup, configuration, and execution steps.
    -->
Para se aceder ao projeto desenvolvido, terá que ter acesso a este repositório para 
posteriormente conseguir abrir o projeto no IDE Android Studio e executa-lo num emulador. Neste projeto
foi utilizado o dispositivo Pixel Pro 9.

---

# Development Process
## 12. Version Control and Commit History
<!-- Describe how version control was used. The commit history must reflect
    continuous work (not only final commits). -->

No momento em que se deu início ao desenvolvimento da aplicação, a aluna não se tinha apercebido de 
que também para as aplicações Android, era necessário um repositório, então devido a essa falha não existem
muitos registos de controlo de versões.

## 13. Difficulties and Lessons Learned
<!-- Main challenges, mistakes, insights, and skills acquired during the assignment.
    -->

No modo landscape a toolBar não preenche o ecrã na sua totalidade. Pensa-se que se deva ao facto de
ter sido alterado o seu tema e a sua cor, e não se conseguiu resolver sem ter que recorrer totalmente
à IA, e devido a esse aspeto, optou-se por não corrigir e investigar melhor o sucedido numa aplicação
futura.

## 14. Future Improvements
<!-- Possible extensions, optimizations, or features that could be added in future
work. -->

- O modo landscape pode ser melhorado, ao perceber melhor como é que funciona a organização das
componentes nos espaço, em conjunto com as suas constraints;

Neste contexto de desenvolvimento de aplicações existe um mundo de personalizações, e pretende-se 
daqui para a frente conseguir desenvolver aplicações funcionais e visualmente engraçadas.

---
## 15. AI Usage Disclosure (Mandatory)
<!-- List all AI tools used (e.g., ChatGPT, Copilot, etc.), how they were used, and
    confirmation that you remain responsible for all content. -->

- **LLM Utilizado:** DeepSeek.
- **Como foi Utilizado:** Para a realização de algumas secções do presente relatório.
- **Responsabilidade:** Eu, aluna Renata Góis (A51038), sou totalmente responsável pelo conteúdo 
apresentado e submetido neste trabalho.