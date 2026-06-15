# Construção do `index.html`

Depois das páginas pessoais estarem aceites no `main`, a equipa constrói o `index.html` em conjunto.

O trabalho está dividido em três sessões. Cada sessão tem um responsável principal e termina com Pull Request.

Resultado esperado:

- `index.html` com apresentação da equipa;
- menu com links para todas as páginas pessoais;
- lista de membros;
- secções sobre o projeto e o trabalho da equipa;
- lema final escolhido pela equipa;
- pelo menos 8 commits relacionados com o `index.html`;
- Pull Requests pequenos e fáceis de rever.

Regra importante:

- A Sessão 2 só começa depois do Pull Request da Sessão 1 estar aceite.
- A Sessão 3 só começa depois do Pull Request da Sessão 2 estar aceite.
- O único conflito esperado é o conflito do lema, na Sessão 3.

---

## Esqueleto HTML a usar nas etapas

As novas partes do `index.html` devem ser criadas dentro de `<main>`, usando secções com a classe `cartao`.

Esqueleto de uma secção simples:

```html
<section class="cartao">
  <h2>Título da secção</h2>
  <p>Primeiro parágrafo.</p>
  <p>Segundo parágrafo.</p>
</section>
```

Esqueleto de uma secção com lista:

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

Esqueleto de um link:

```html
<a href="ficheiro.html">Texto do link</a>
```

No fim de cada etapa:

1. testar o `index.html` no browser;
2. rever as alterações;
3. criar um commit só com essa etapa.

Os comandos não são repetidos em cada etapa de propósito. A equipa deve escolher os comandos adequados.

Comandos que podem ser úteis:

```bash
git switch main
git pull
git switch -c nome-do-branch
git status
git diff
git add index.html
git commit -m "Mensagem clara em portugues"
git push -u origin nome-do-branch
git log --oneline
```

---

## Sessão 1 — Apresentação da equipa

Responsável sugerido: Formando 1.

Objetivo: melhorar o topo e criar as primeiras secções de conteúdo do `index.html`.

Branch sugerido:

```text
feature/index-apresentacao
```

Esta sessão deve criar 3 commits.

---

### Etapa I1 — Título e apresentação inicial

Objetivo: identificar o projeto e apresentar a equipa.

Conteúdo a criar ou rever:

- `<title>` com o nome `projeto617`;
- `h1` com o nome `projeto617`;
- manter a linha do lema sem alterações;
- substituir o texto temporário da secção `Equipa`;
- escrever 2 parágrafos sobre a equipa.

Não alterar ainda esta linha:

```html
<p class="lema">Lema a decidir pela equipa</p>
```

Essa linha será usada na Sessão 3 para criar o conflito controlado.

Esqueleto esperado:

```html
<section class="cartao">
  <h2>Equipa</h2>
  <p>Frase sobre quem é a equipa.</p>
  <p>Frase sobre como a equipa vai trabalhar no projeto.</p>
</section>
```

Pistas de escrita:

- Quem faz parte da equipa?
- O que a equipa vai construir?
- Porque estão a usar Git e GitHub?

Commit da etapa:

- criar um commit só com esta alteração;
- mensagem sugerida: `Melhora apresentacao inicial do index`.

---

### Etapa I2 — Secção Como trabalhamos

Objetivo: explicar como a equipa organiza o trabalho.

Conteúdo a criar:

- nova secção com o título `Como trabalhamos`;
- 1 ou 2 parágrafos;
- lista com 3 formas de trabalho.

Esqueleto esperado:

```html
<section class="cartao">
  <h2>Como trabalhamos</h2>
  <p>Frase sobre a organização da equipa.</p>
  <p>Frase sobre a importância de rever alterações.</p>
  <ul class="top3">
    <li>Primeira regra de trabalho</li>
    <li>Segunda regra de trabalho</li>
    <li>Terceira regra de trabalho</li>
  </ul>
</section>
```

Pistas para a lista:

- trabalhar em branches;
- fazer commits pequenos;
- rever Pull Requests;
- testar no browser;
- manter o `main` funcional.

Commit da etapa:

- criar um commit só com esta secção;
- mensagem sugerida: `Explica metodo de trabalho da equipa`.

---

### Etapa I3 — Secção Objetivo do projeto

Objetivo: explicar o objetivo do projeto.

Conteúdo a criar:

- nova secção com o título `Objetivo do projeto`;
- 2 parágrafos;
- pelo menos um parágrafo com `class="texto-destaque"`.

Esqueleto esperado:

```html
<section class="cartao">
  <h2>Objetivo do projeto</h2>
  <p>Frase sobre o objetivo geral do projeto.</p>
  <p class="texto-destaque">Frase em destaque sobre Git, GitHub e colaboração.</p>
</section>
```

Pistas de escrita:

- O que a equipa vai praticar?
- Porque é importante trabalhar com branches?
- O que se espera aprender com Pull Requests e conflitos?

Commit da etapa:

- criar um commit só com esta secção;
- mensagem sugerida: `Adiciona objetivo do projeto`.

---

### Pull Request da Sessão 1

Depois das 3 etapas:

1. confirmar que existem 3 commits no branch;
2. enviar o branch para o GitHub;
3. abrir Pull Request;
4. usar um título claro;
5. pedir revisão a um colega.

Título sugerido:

```text
Melhora apresentação do index
```

Depois do merge, todos atualizam o `main` antes de continuar.

---

## Sessão 2 — Menu, membros e páginas

Responsável sugerido: Formando 2.

Objetivo: ligar o `index.html` às páginas pessoais e completar a navegação.

Branch sugerido:

```text
feature/index-menu
```

Esta sessão deve criar 3 commits.

---

### Etapa I4 — Menu de navegação

Objetivo: permitir navegar da página inicial para as páginas pessoais.

Conteúdo a alterar:

- manter o link para `index.html`;
- adicionar um link para cada página pessoal;
- remover o comentário temporário do menu.

Esqueleto esperado:

```html
<nav>
  <ul class="menu">
    <li><a href="index.html">Início</a></li>
    <li><a href="membro-ana.html">Ana</a></li>
    <li><a href="membro-bruno.html">Bruno</a></li>
    <li><a href="membro-carla.html">Carla</a></li>
  </ul>
</nav>
```

Ajustar os nomes e ficheiros ao grupo.

Se o grupo tiver 2 elementos, remover o terceiro link.

Commit da etapa:

- testar todos os links no browser;
- criar um commit só com o menu;
- mensagem sugerida: `Adiciona links das paginas pessoais`.

---

### Etapa I5 — Secção Membros

Objetivo: apresentar os membros da equipa no conteúdo da página.

Conteúdo a criar:

- nova secção com o título `Membros`;
- 1 parágrafo introdutório;
- lista com os membros da equipa.

Esqueleto esperado:

```html
<section class="cartao">
  <h2>Membros</h2>
  <p>Frase sobre as páginas pessoais criadas pela equipa.</p>
  <ul class="top3">
    <li>Nome do primeiro membro e respetiva página</li>
    <li>Nome do segundo membro e respetiva página</li>
    <li>Nome do terceiro membro e respetiva página</li>
  </ul>
</section>
```

Pistas de escrita:

- Quem criou cada página?
- Que ficheiro corresponde a cada membro?
- O que o visitante pode encontrar nessas páginas?

Commit da etapa:

- criar um commit só com esta secção;
- mensagem sugerida: `Adiciona lista de membros`.

---

### Etapa I6 — Secção Páginas do projeto

Objetivo: listar as páginas do projeto com links.

Conteúdo a criar:

- nova secção com o título `Páginas do projeto`;
- 1 parágrafo introdutório;
- lista com links para as páginas pessoais.

Esqueleto esperado:

```html
<section class="cartao">
  <h2>Páginas do projeto</h2>
  <p>Frase sobre a navegação entre páginas.</p>
  <ul class="top3">
    <li><a href="membro-ana.html">Página pessoal da Ana</a></li>
    <li><a href="membro-bruno.html">Página pessoal do Bruno</a></li>
    <li><a href="membro-carla.html">Página pessoal da Carla</a></li>
  </ul>
</section>
```

Ajustar nomes e ficheiros ao grupo.

Commit da etapa:

- testar todos os links da secção;
- criar um commit só com esta secção;
- mensagem sugerida: `Adiciona lista de paginas do projeto`.

---

### Pull Request da Sessão 2

Depois das 3 etapas:

1. confirmar que existem 3 commits no branch;
2. enviar o branch para o GitHub;
3. abrir Pull Request;
4. usar um título claro;
5. pedir revisão a um colega.

Título sugerido:

```text
Adiciona menu e páginas ao index
```

Depois do merge, todos atualizam o `main` antes de continuar.

---

## Sessão 3 — Lema, conflito controlado e fecho do index

Responsável sugerido: Formando 3. Se o grupo tiver 2 elementos, escolham um responsável.

Objetivo: decidir o lema final, resolver um conflito real e fechar o conteúdo do `index.html`.

Esta sessão tem duas partes:

- propostas de lema em paralelo, para criar um conflito controlado;
- melhoria final do `index.html`, feita depois do conflito estar resolvido.

---

## Parte A — Propostas de lema em paralelo

Todos os membros fazem esta parte ao mesmo tempo.

Regra para manter o conflito simples:

- nos branches de lema, alterar apenas a linha `<p class="lema">`;
- não alterar menu, secções, listas ou rodapé nesses branches.

Branch sugerido:

```text
feature/lema-nome
```

Linha a alterar:

```html
<p class="lema">Lema a decidir pela equipa</p>
```

Cada membro substitui o texto por uma proposta diferente.

Exemplo:

```html
<p class="lema">Aprender juntos, versionar melhor</p>
```

Commit da etapa:

- testar o `index.html`;
- criar um commit só com a proposta de lema;
- mensagem sugerida: `Propoe lema da equipa`.

Depois:

1. cada membro envia o seu branch;
2. cada membro abre Pull Request;
3. um colega revê e faz merge do primeiro Pull Request;
4. o segundo Pull Request deve apresentar conflito;
5. se o grupo tiver 3 elementos, o terceiro Pull Request também pode apresentar conflito.

---

## Parte B — Resolução do conflito

O conflito é resolvido pelo autor do Pull Request que ficou com conflito, porque é esse formando que tem o branch no seu computador.

Não tem de ser o owner do repositório. O owner só precisa de intervir se for necessário por permissões do GitHub.

Aqui os comandos são indicados porque a resolução de conflitos é uma parte sensível.

1. Mudar para o branch com conflito:

   ```bash
   git switch feature/lema-nome
   ```

2. Atualizar esse branch com o `main`:

   ```bash
   git pull origin main
   ```

3. Abrir `index.html`. O Git vai mostrar marcas parecidas com estas:

   ```html
   <<<<<<< HEAD
   <p class="lema">Lema que já entrou no main</p>
   =======
   <p class="lema">Outro lema proposto</p>
   >>>>>>> feature/lema-nome
   ```

4. Apagar as marcas:

   ```text
   <<<<<<<
   =======
   >>>>>>>
   ```

5. Decidir em equipa qual frase fica.

6. O resultado final deve ter apenas uma linha:

   ```html
   <p class="lema">Lema final decidido pela equipa</p>
   ```

7. Testar `index.html` no browser.

8. Criar um commit para a resolução do conflito.

   Mensagem sugerida:

   ```text
   Resolve conflito do lema
   ```

9. Enviar o branch atualizado.

10. Confirmar no GitHub que o Pull Request ficou sem conflito.

11. Um colega revê e faz merge.

12. Se ainda existir outro Pull Request de lema com conflito, repetir esta parte.

Depois de todos os Pull Requests de lema estarem aceites, todos atualizam o `main`.

---

## Parte C — Melhoria final do `index.html`

Esta parte é feita depois dos Pull Requests de lema estarem resolvidos.

Só uma pessoa abre este Pull Request, de preferência o responsável da Sessão 3.

Branch sugerido:

```text
feature/index-fecho
```

---

### Etapa I7 — Secção Aprendizagens da equipa

Objetivo: resumir o que a equipa aprendeu.

Conteúdo a criar:

- nova secção com o título `Aprendizagens da equipa`;
- 2 parágrafos.

Esqueleto esperado:

```html
<section class="cartao">
  <h2>Aprendizagens da equipa</h2>
  <p>Frase sobre o que a equipa aprendeu com Git e GitHub.</p>
  <p>Frase sobre revisão, colaboração ou conflitos.</p>
</section>
```

Pistas de escrita:

- O que correu bem?
- O que foi mais difícil?
- O que aprenderam sobre trabalho em equipa?

Commit da etapa:

- criar um commit só com esta secção;
- mensagem sugerida: `Adiciona aprendizagens da equipa`.

---

### Etapa I8 — Secção Próximos passos

Objetivo: fechar o conteúdo do `index.html`.

Conteúdo a criar:

- nova secção com o título `Próximos passos`;
- 2 parágrafos;
- pelo menos um parágrafo com `class="texto-destaque"`.

Esqueleto esperado:

```html
<section class="cartao">
  <h2>Próximos passos</h2>
  <p>Frase sobre o que falta fazer antes da entrega final.</p>
  <p class="texto-destaque">Frase em destaque sobre a entrega final do projeto.</p>
</section>
```

Pistas de escrita:

- rever o site;
- atualizar o README;
- publicar ou confirmar o GitHub Pages;
- preparar a apresentação final.

Commit da etapa:

- testar todos os links do `index.html`;
- criar um commit só com esta secção;
- mensagem sugerida: `Adiciona proximos passos ao index`.

---

### Pull Request da melhoria final

Depois das etapas I7 e I8:

1. confirmar que existem commits separados para cada etapa;
2. enviar o branch para o GitHub;
3. abrir Pull Request;
4. usar um título claro;
5. pedir revisão a um colega.

Título sugerido:

```text
Finaliza conteúdo do index
```

Depois do merge, todos atualizam o `main`.

---

## Checklist final do `index.html`

Antes de avançar para o README final, confirmar:

- o `index.html` abre no browser;
- o menu tem link para `index.html` e para todas as páginas pessoais;
- todos os links funcionam;
- existe uma secção `Equipa`;
- existe uma secção `Como trabalhamos`;
- existe uma secção `Objetivo do projeto`;
- existe uma secção `Membros`;
- existe uma secção `Páginas do projeto`;
- existe uma secção `Aprendizagens da equipa`;
- existe uma secção `Próximos passos`;
- existe um lema final;
- existem pelo menos 8 commits relacionados com o `index.html`;
- não existem marcas de conflito no ficheiro;
- o CSS não foi alterado.

Marcas de conflito que não podem ficar no ficheiro:

```text
<<<<<<<
=======
>>>>>>>
```
