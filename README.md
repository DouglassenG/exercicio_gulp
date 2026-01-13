# 🥤 Gulp - Automação de Tarefas Frontend

![Status](https://img.shields.io/badge/Status-Finalizado-green)
![Gulp](https://img.shields.io/badge/Build_Tool-Gulp.js-red?logo=gulp&logoColor=white)
![SASS](https://img.shields.io/badge/Style-SASS-pink?logo=sass&logoColor=white)
![JavaScript](https://img.shields.io/badge/Code-JavaScript-yellow?logo=javascript&logoColor=white)

> Um projeto focado na produtividade do desenvolvedor e performance da aplicação, utilizando Streams do Node.js para automatizar tarefas repetitivas.

## 🎯 Motivação e Propósito

No desenvolvimento profissional, entregar arquivos "crus" (comentários, espaços em branco, imagens pesadas) prejudica a performance do site. O propósito deste repositório é implementar um **Build System** eficiente.

Este projeto resolve o problema da otimização manual. Ele configura o Gulp para "assistir" os arquivos de desenvolvimento e, automaticamente, gerar versões de produção leves e compiladas, garantindo carregamento rápido e código organizado.

## 🛠️ Tecnologias Utilizadas

A arquitetura do projeto utiliza o ecossistema Node.js:

* **[Gulp.js](https://gulpjs.com/):** Toolkit para automatização de tarefas baseada em streams (leitura/escrita de arquivos em memória).
* **[SASS (Dart Sass)](https://sass-lang.com/):** Pré-processador CSS para estilos avançados.
* **Plugins Gulp:**
    * `gulp-sass`: Compilação de .scss para .css.
    * `gulp-uglify`: Ofuscação e minificação de JavaScript.
    * `gulp-imagemin`: Compressão de imagens (PNG/JPEG) sem perda visível de qualidade.
* **[Node.js & NPM](https://nodejs.org/):** Gerenciamento de dependências.

## ✨ Funcionalidades

O arquivo `gulpfile.js` foi configurado para executar as seguintes tarefas:

1.  **Compilação de Estilos:** Transforma arquivos SASS da pasta `src` em CSS padrão na pasta `dist`.
2.  **Otimização de Scripts:** Remove espaços e renomeia variáveis (Uglify) para reduzir o tamanho dos arquivos JS.
3.  **Compressão de Assets:** Reduz o peso das imagens automaticamente ao movê-las para a pasta de distribuição.
4.  **Watch Mode:** Monitora alterações nos arquivos fonte e executa as tarefas automaticamente em tempo real.

## 📦 Instalação e Configuração

Como este projeto depende de módulos do Node, siga os passos abaixo para configurar o ambiente.

### Pré-requisitos
* **Node.js** (Versão LTS recomendada) instalado.
* **Git** instalado.

### Passo a Passo

1.  **Clone o repositório:**
    ```bash
    git clone [https://github.com/DouglassenG/exercicio_gulp.git](https://github.com/DouglassenG/exercicio_gulp.git)
    ```

2.  **Acesse o diretório:**
    ```bash
    cd exercicio_gulp
    ```

3.  **Instale as dependências:**
    O comando abaixo lerá o arquivo `package.json` e instalará o Gulp e seus plugins na pasta `node_modules`.
    ```bash
    npm install
    ```

4.  **Execute o Build:**
    Para rodar todas as tarefas e processar os arquivos:
    ```bash
    npm run build
    # ou
    gulp
    ```

## 💻 Uso e Exemplos

A estrutura do projeto separa claramente o ambiente de desenvolvimento (`src`) do produto final (`dist`).

**Estrutura de Pastas:**
```text
exercicio_gulp/
├── src/              # Arquivos Fontes (Onde você codifica)
│   ├── styles/       # .scss
│   ├── scripts/      # .js
│   └── images/       # Imagens originais
├──
