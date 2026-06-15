# Página pessoal

Cada formando cria uma página pessoal em HTML.

Esta página serve para:

- praticar a estrutura básica de uma página HTML;
- escrever conteúdo próprio;
- trabalhar num branch individual;
- fazer vários commits pequenos;
- abrir um Pull Request simples, fácil de rever.

---

## Nome do ficheiro

O ficheiro deve chamar-se:

```text
membro-nome.html
```

Substitui `nome` pelo teu primeiro nome, sem acentos e em minúsculas.

Exemplos:

```text
membro-ana.html
membro-bruno.html
membro-carla.html
```

Usa o ficheiro `modelo.html` como base.

Não alteres `css/style.css`. O CSS já está pronto.

---

## Resultado esperado

No fim desta tarefa, a tua página deve ter:

- um ficheiro HTML novo;
- o teu nome no `<title>`;
- um `h1` com o teu nome;
- várias secções com `class="cartao"`;
- parágrafos escritos por ti;
- pelo menos uma lista com `ul` e `li`;
- um link para voltar ao `index.html`;
- pelo menos 8 commits no branch da tua página;
- um Pull Request aberto para revisão.

---

## Forma de trabalho

Trabalha sempre no branch da tua página.

Nome sugerido para o branch:

```text
feature/pagina-nome
```

Exemplo:

```text
feature/pagina-ana
```

Não cries a página toda de uma vez. Divide o trabalho em etapas pequenas.

Depois de cada etapa:

1. abre a página no browser;
2. confirma que o conteúdo aparece corretamente;
3. verifica as alterações;
4. faz um commit com uma mensagem clara.

Os comandos não estão repetidos em cada etapa de propósito. Deves escolher os comandos adequados ao momento.

Comandos que podem ser úteis:

```bash
git switch main
git pull
git switch -c feature/pagina-nome
git status
git diff
git add membro-nome.html
git commit -m "Mensagem clara em portugues"
git push -u origin feature/pagina-nome
git log --oneline
```

---

## Estrutura da página

A página deve ser construída por etapas.

Cada etapa acrescenta uma parte nova da página.

No `modelo.html`, a estrutura principal já existe:

```html
<header>
  <!-- Cabeçalho da página -->
</header>

<nav>
  <!-- Menu de navegação -->
</nav>

<main>
  <!-- Conteúdo principal da página -->
</main>

<footer>
  <!-- Rodapé -->
</footer>
```

Regras importantes:

- o `<title>` fica dentro de `<head>`;
- o `h1` fica dentro de `<header>`;
- as secções da página ficam dentro de `<main>`;
- cada nova secção deve usar `<section class="cartao">`;
- listas usam `<ul>` e, dentro dela, vários `<li>`;
- links usam `<a href="destino.html">Texto do link</a>`;
- não apagar as tags principais: `html`, `head`, `body`, `header`, `nav`, `main` e `footer`.

Modelo para uma secção simples:

```html
<section class="cartao">
  <h2>Título da secção</h2>
  <p>Primeiro parágrafo da secção.</p>
  <p>Segundo parágrafo da secção.</p>
</section>
```

Modelo para uma secção com lista:

```html
<section class="cartao">
  <h2>Título da secção</h2>
  <p>Frase introdutória antes da lista.</p>
  <ul class="top3">
    <li>Primeiro item</li>
    <li>Segundo item</li>
    <li>Terceiro item</li>
  </ul>
</section>
```

---

## Etapa 1 — Cabeçalho

Objetivo: criar o ficheiro e identificar a página.

Conteúdo esperado:

- copiar a estrutura de `modelo.html`;
- alterar o `<title>` para o teu nome;
- adicionar um `h1` com o teu nome;
- adicionar uma frase curta no cabeçalho.

Sugestões para a frase curta:

- uma frase sobre o que estás a aprender;
- uma frase sobre o teu objetivo no projeto;
- uma frase que te represente enquanto formando.

Exemplo de estrutura:

```html
<header>
  <h1 class="titulo-principal">Nome</h1>
  <p class="lema">Frase curta sobre ti ou sobre o projeto.</p>
</header>
```

Nesta etapa, também deves alterar o `<title>`:

```html
<title>Nome</title>
```

Commit da etapa:

- criar um commit só com o ficheiro e o cabeçalho;
- mensagem sugerida: `Cria cabecalho da pagina pessoal`.

---

## Etapa 2 — Sobre mim

Objetivo: apresentar-te de forma simples.

Conteúdo esperado:

- criar uma secção com o título `Sobre mim`;
- escrever 2 ou 3 parágrafos;
- usar pelo menos um parágrafo com a classe `texto-destaque`.

Pistas de escrita:

- Quem és?
- Porque estás neste curso?
- Que tipo de atividades gostas de fazer?
- O que esperas aprender com este projeto?

Evita frases genéricas como “Gosto de informática”. Escreve frases mais concretas.

Estrutura HTML sugerida:

```html
<section class="cartao">
  <h2>Sobre mim</h2>
  <p>Primeira frase sobre ti.</p>
  <p>Segunda frase sobre ti.</p>
  <p class="texto-destaque">Frase em destaque sobre este projeto.</p>
</section>
```

Commit da etapa:

- criar um commit só com a secção `Sobre mim`;
- mensagem sugerida: `Adiciona secao sobre mim`.

---

## Etapa 3 — Percurso

Objetivo: explicar um pouco do teu percurso.

Conteúdo esperado:

- criar uma secção com o título `Percurso`;
- escrever 2 parágrafos.

Pistas de escrita:

- Que contacto já tiveste com tecnologia?
- Já tinhas usado HTML, Git ou GitHub?
- Que parte do curso tem sido mais desafiante?
- Que área gostarias de explorar melhor?

Estrutura HTML sugerida:

```html
<section class="cartao">
  <h2>Percurso</h2>
  <p>Frase sobre o teu percurso de aprendizagem.</p>
  <p>Frase sobre uma área que queres explorar melhor.</p>
</section>
```

Commit da etapa:

- criar um commit só com a secção `Percurso`;
- mensagem sugerida: `Adiciona percurso pessoal`.

---

## Etapa 4 — O que estou a aprender

Objetivo: ligar a tua página aos conteúdos da UC00617.

Conteúdo esperado:

- criar uma secção com o título `O que estou a aprender`;
- escrever 1 parágrafo introdutório;
- criar uma lista com 3 aprendizagens.

Pistas para a lista:

- branches;
- commits;
- Pull Requests;
- revisão por colegas;
- resolução de conflitos;
- HTML básico;
- organização de ficheiros.

Cada item da lista deve ser escrito por palavras tuas.

Estrutura HTML sugerida:

```html
<section class="cartao">
  <h2>O que estou a aprender</h2>
  <p>Frase introdutória sobre as tuas aprendizagens.</p>
  <ul class="top3">
    <li>Primeira aprendizagem</li>
    <li>Segunda aprendizagem</li>
    <li>Terceira aprendizagem</li>
  </ul>
</section>
```

Commit da etapa:

- criar um commit só com a secção `O que estou a aprender`;
- mensagem sugerida: `Descreve aprendizagens da UC`.

---

## Etapa 5 — Ferramentas usadas

Objetivo: identificar as ferramentas usadas no projeto.

Conteúdo esperado:

- criar uma secção com o título `Ferramentas usadas`;
- escrever 1 parágrafo;
- criar uma lista com 3 ferramentas.

Pistas para a lista:

- VS Code;
- GitHub Desktop;
- Git;
- GitHub;
- browser;
- GitHub Pages.

Não precisas de listar todas as ferramentas. Escolhe as que usaste mesmo.

Estrutura HTML sugerida:

```html
<section class="cartao">
  <h2>Ferramentas usadas</h2>
  <p>Frase sobre como usaste ferramentas no projeto.</p>
  <ul class="top3">
    <li>Primeira ferramenta</li>
    <li>Segunda ferramenta</li>
    <li>Terceira ferramenta</li>
  </ul>
</section>
```

Commit da etapa:

- criar um commit só com a secção `Ferramentas usadas`;
- mensagem sugerida: `Adiciona ferramentas usadas`.

---

## Etapa 6 — Comandos ou ações praticadas

Objetivo: mostrar o que praticaste durante o trabalho.

Conteúdo esperado:

- criar uma secção com o título `Comandos praticados` ou `Ações praticadas`;
- criar uma lista com 3 itens.

Pistas para a lista:

- verificar alterações;
- criar commits;
- atualizar o `main`;
- criar branches;
- enviar um branch para o GitHub;
- abrir Pull Requests;
- testar a página no browser.

Podes escrever comandos concretos ou ações em linguagem natural.

Estrutura HTML sugerida:

```html
<section class="cartao">
  <h2>Comandos praticados</h2>
  <p>Frase sobre o que praticaste durante o trabalho.</p>
  <ul class="top3">
    <li>Primeiro comando ou ação</li>
    <li>Segundo comando ou ação</li>
    <li>Terceiro comando ou ação</li>
  </ul>
</section>
```

Commit da etapa:

- criar um commit só com a secção de comandos ou ações praticadas;
- mensagem sugerida: `Lista comandos praticados`.

---

## Etapa 7 — O meu Top 3

Objetivo: acrescentar uma parte mais pessoal.

Conteúdo esperado:

- criar uma secção com o título `O meu Top 3`;
- escrever 1 frase introdutória;
- criar uma lista com 3 itens.

Pistas para o Top 3:

- ferramentas preferidas;
- temas que gostaste de aprender;
- jogos;
- filmes;
- músicas;
- comidas;
- linguagens;
- áreas de interesse.

Escolhe um tema e mantém os 3 itens dentro desse tema.

Estrutura HTML sugerida:

```html
<section class="cartao">
  <h2>O meu Top 3</h2>
  <p>Frase introdutória sobre o tema escolhido.</p>
  <ul class="top3">
    <li>Primeiro item</li>
    <li>Segundo item</li>
    <li>Terceiro item</li>
  </ul>
</section>
```

Commit da etapa:

- criar um commit só com a secção `O meu Top 3`;
- mensagem sugerida: `Adiciona top 3 pessoal`.

---

## Etapa 8 — Objetivos e navegação

Objetivo: fechar a página.

Conteúdo esperado:

- criar uma secção com o título `Objetivos`;
- escrever 2 parágrafos sobre o que queres melhorar;
- criar uma secção de navegação;
- adicionar um link para `index.html`.

Pistas para os objetivos:

- ganhar autonomia com Git;
- escrever HTML com mais segurança;
- perceber melhor Pull Requests;
- resolver conflitos sem receio;
- trabalhar melhor em equipa.

O link de regresso deve usar `href="index.html"`.

Estrutura HTML sugerida para os objetivos:

```html
<section class="cartao">
  <h2>Objetivos</h2>
  <p>Primeiro objetivo que queres melhorar.</p>
  <p class="texto-destaque">Segundo objetivo em destaque.</p>
</section>
```

Estrutura HTML sugerida para a navegação:

```html
<section class="cartao">
  <h2>Navegação</h2>
  <p><a class="link-voltar" href="index.html">Voltar ao início</a></p>
</section>
```

Commit da etapa:

- criar um commit só com os objetivos e a navegação;
- mensagem sugerida: `Adiciona objetivos e link de regresso`.

---

## Revisão antes do Pull Request

Antes de abrir o Pull Request, confirma:

- o ficheiro tem o nome correto;
- o `<title>` tem o teu nome;
- existe um `h1` com o teu nome;
- existem várias secções com `class="cartao"`;
- os textos foram escritos por ti;
- não há frases temporárias;
- existe pelo menos uma lista;
- existe um link para `index.html`;
- a página abre no browser;
- o link para `index.html` funciona;
- o CSS não foi alterado;
- existem pelo menos 8 commits no branch.

---

## Pull Request da página

Depois de terminar a página:

1. envia o branch para o GitHub;
2. abre um Pull Request;
3. usa um título claro;
4. resume o que criaste;
5. indica como testar a página;
6. espera até todos os membros terem aberto o Pull Request da sua página;
7. revê o Pull Request de um colega;
8. garante que não fazes merge do teu próprio Pull Request.

Título sugerido:

```text
Cria página pessoal de Nome
```

Na descrição do Pull Request, deves indicar:

- nome do ficheiro criado;
- principais secções adicionadas;
- confirmação de que a página foi testada no browser;
- confirmação de que o link para `index.html` funciona.
