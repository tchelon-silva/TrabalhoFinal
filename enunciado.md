# Enunciado — projeto617
### Trabalho de grupo · Git + GitHub · UC00617

## Contexto

Este trabalho final chama-se sempre **projeto617**.

O objetivo é construir um pequeno projeto web de equipa usando Git e GitHub. O foco principal é a colaboração: branches, commits, Pull Requests, revisão por colegas, resolução de conflitos e publicação do projeto final.

O HTML pedido é básico. Devem usar elementos simples como `h1`, `h2`, `p`, `ul`, `li`, `a`, `header`, `nav`, `main`, `section` e `footer`.

O CSS é fornecido pelo formador e não deve ser alterado.

---

## Grupos

- 2 a 3 elementos por grupo.
- Cada elemento trabalha no seu computador.
- Todos devem contribuir no repositório.
- Ninguém faz merge do seu próprio Pull Request.

---

## Starter fornecido

O projeto começa com poucos ficheiros:

```text
projeto617/
├── index.html        → página inicial com estrutura básica
├── modelo.html       → template HTML5 para criar novas páginas
├── css/style.css     → estilo fornecido pelo formador
├── enunciado.md      → enunciado geral do trabalho
├── tarefas/          → guias de trabalho
├── .gitignore        → ficheiros ignorados pelo Git
└── README.md         → descrição do projeto
```

Não existem páginas pessoais criadas pelos formandos no início. Cada formando cria a sua página de raiz, usando `modelo.html` como base e seguindo o guia `tarefas/pagina-pessoal.md`.

---

## O que a equipa vai construir

No fim, o projeto deve ter:

- `index.html` com apresentação da equipa e várias secções sobre o projeto e o método de trabalho
- Uma página pessoal completa por formando, com o nome `membro-nome.html`
- Menu de navegação entre a página inicial e as páginas pessoais
- Lista de membros no `index.html`
- Um lema escolhido pela equipa
- Conteúdo simples em HTML nas páginas pessoais, organizado em várias secções
- README atualizado
- Projeto publicado com GitHub Pages

---

## Rotina de trabalho

Antes de criar um branch novo para uma tarefa, cada membro atualiza o `main` local:

```bash
git switch main
git pull
```

Se o formando já está a continuar trabalho no mesmo branch, não precisa de repetir este passo.

Antes de cada commit, cada membro verifica o que mudou:

```bash
git status
git diff
```

Antes de abrir um Pull Request:

- Abrir o projeto no browser.
- Testar os links alterados.
- Confirmar que a página continua legível.

Em todos os commits:

- Usar mensagens claras em português.
- Fazer commits pequenos e relacionados com uma tarefa.

---

## Carga de trabalho esperada

Este projeto não deve ser feito numa única alteração grande.

Cada página pessoal deve ter:

- pelo menos 8 etapas;
- pelo menos 8 commits no mesmo branch;
- várias secções de conteúdo;
- um único Pull Request no fim.

O `index.html` deve ser construído em sessões:

- Sessão 1: apresentação da equipa, com 3 commits;
- Sessão 2: menu, membros e páginas, com 3 commits;
- Sessão 3: lema, conflito controlado e fecho do `index.html`.

Na Sessão 3, cada proposta de lema tem um Pull Request simples. Depois do conflito estar resolvido, existe ainda um Pull Request final para fechar o conteúdo do `index.html`.

Os Pull Requests foram pensados para serem fáceis de resolver:

- as páginas pessoais são ficheiros diferentes;
- as sessões do `index.html` são feitas por ordem;
- o único conflito esperado é o conflito do lema, numa única linha.

---

## Regras obrigatórias

1. O repositório chama-se `projeto617`.
2. O trabalho normal é feito em branch, não diretamente no `main`.
3. Cada alteração relevante deve ter um Pull Request.
4. O autor de um Pull Request não pode fazer merge do seu próprio Pull Request.
5. Cada Pull Request deve ser revisto por um colega.
6. O `main` deve estar sempre funcional.
7. O CSS fornecido não deve ser alterado.
8. O histórico deve mostrar colaboração real entre os membros.

Exceções permitidas:

- Primeiro envio do starter para o GitHub.
- Pequenas correções finais combinadas com o formador.

---

# Parte 1 — Preparação do repositório

## Setup inicial

Antes de criar Issues ou editar páginas, a equipa segue o guia `tarefas/setup.md`.

No fim desta parte, o repositório `projeto617` deve existir no GitHub, a branch principal deve chamar-se `main` e todos os membros devem ter acesso local ao projeto.

---

# Parte 2 — Planeamento no GitHub

Antes de editar ficheiros, a equipa cria Issues no GitHub.

Criem, no mínimo:

- Uma Issue para cada página pessoal
- Uma Issue para a apresentação da equipa no `index.html`
- Uma Issue para o menu e a lista de membros no `index.html`
- Uma Issue para o lema da equipa e o conflito obrigatório
- Uma Issue para atualizar o README
- Uma Issue para publicação com GitHub Pages

Cada Issue deve ter:

- Título claro
- Responsável
- Label adequada, por exemplo `enhancement` ou `documentation`

Cada membro deve ficar responsável por pelo menos uma Issue e deve indicar na Issue qual o guia `.md` que vai seguir.

Durante o projeto:

- cada Pull Request deve estar relacionado com uma Issue;
- a equipa deve fechar as Issues quando o trabalho correspondente estiver aceite no `main`;
- no fim, deve ser possível perceber pelas Issues como o trabalho foi planeado e acompanhado.

---

# Parte 3 — Desenvolvimento guiado

O desenvolvimento está dividido em guias `.md`, por tipo de tarefa.

Os guias estão na pasta `tarefas/`:

```text
tarefas/
├── setup.md
├── pagina-pessoal.md
├── index.md
└── readme-final.md
```

Primeiro, todos seguem `setup.md`.

Depois, a distribuição sugerida é:

- Cada formando segue `pagina-pessoal.md` para criar a sua própria página.
- A equipa segue `index.md` para construir o `index.html` em três sessões.
- A equipa segue `readme-final.md` no fim do projeto.

Na página pessoal, cada formando trabalha num branch próprio.

Dentro desse branch, o formando faz várias etapas. Cada etapa deve terminar com revisão das alterações e um commit claro.

No fim da página pessoal, cada membro faz push do seu branch e abre **um Pull Request da sua página**.

Este é o primeiro momento em que devem existir vários Pull Requests ao mesmo tempo: um por cada membro. A equipa só começa as revisões quando todos os membros tiverem o seu Pull Request aberto.

Depois, cada Pull Request é revisto e aceite por um colega.

Depois das páginas pessoais estarem aceites no `main`, a equipa segue `tarefas/index.md`. O `index.html` é construído em três sessões, com Pull Requests pequenos e feitos por ordem.

Os formandos devem seguir as instruções HTML dos guias. As instruções são intencionalmente detalhadas para apoiar quem ainda só conhece HTML básico.

No fim desta parte:

- Cada membro criou a sua página pessoal.
- Cada página foi construída em pelo menos 8 etapas.
- O histórico mostra vários commits.
- Existem vários Pull Requests abertos em paralelo, um por página.

---

# Parte 4 — Construção conjunta do `index.html`

Depois das páginas pessoais estarem no `main`, a equipa segue o guia `tarefas/index.md`.

No fim desta parte:

- O menu do `index.html` liga todas as páginas criadas.
- O `index.html` apresenta a equipa.
- O `index.html` tem várias secções de conteúdo.
- Os links foram testados no browser.

---

# Parte 5 — Conflito obrigatório

O conflito obrigatório está descrito na Sessão 3 de `tarefas/index.md`.

No fim desta parte:

- O `index.html` tem um único lema final.
- O histórico mostra trabalho paralelo.
- A equipa consegue explicar porque aconteceu o conflito.

---

# Parte 6 — Revisão final do projeto

Antes da publicação, a equipa revê o projeto completo.

Verifiquem:

- O `index.html` abre no browser.
- Todas as páginas criadas abrem no browser.
- Todos os links do menu funcionam.
- Cada página tem título correto no separador do browser.
- Cada página tem conteúdo próprio.
- O CSS fornecido não foi alterado.
- Não há ficheiros de rascunho ou lixo no repositório.
- O `README.md` descreve o projeto e identifica a equipa.

Se forem necessárias correções, devem ser feitas em branch e Pull Request, salvo indicação do formador.

---

# Parte 7 — Publicação e README final

## GitHub Pages

Publicar o projeto com GitHub Pages:

```text
Settings -> Pages -> Deploy from a branch -> main / root
```

O URL esperado terá este formato:

```text
https://UTILIZADOR.github.io/projeto617/
```

## README final

Depois de o projeto estar publicado, adicionar o link do projeto ao topo do `README.md`.

A atualização final do README está detalhada em `tarefas/readme-final.md`.

---

# Entrega

A equipa entrega ao formador:

- Link do repositório GitHub
- Link do projeto publicado
- Lista de Issues criadas e fechadas
- Pull Requests aceites

Não é necessário entregar ficheiros por email ou em `.zip`, salvo indicação do formador. A entrega principal é feita através dos links do GitHub.

---

# Avaliação

A avaliação incide sobre o produto final e sobre o processo de trabalho.

## 1. Organização no GitHub

Será avaliado se:

- o repositório se chama `projeto617`;
- foram criadas Issues no início do projeto;
- as Issues têm responsáveis e títulos claros;
- as Issues foram usadas para acompanhar o trabalho;
- os Pull Requests estão relacionados com as tarefas planeadas.

## 2. Histórico Git

Será avaliado se:

- o trabalho foi feito em branches;
- existem vários commits por página ou etapa;
- as mensagens dos commits são claras e em português;
- o histórico mostra trabalho distribuído pelos membros;
- o `main` se manteve funcional.

## 3. Pull Requests e colaboração

Será avaliado se:

- cada membro abriu Pull Requests;
- os Pull Requests foram revistos por colegas;
- ninguém fez merge do seu próprio Pull Request;
- houve vários Pull Requests em paralelo nas páginas pessoais;
- a equipa resolveu pelo menos um conflito real.

## 4. HTML e conteúdo

Será avaliado se:

- existe uma página pessoal por formando;
- as páginas usam a estrutura HTML indicada;
- o `index.html` liga todas as páginas;
- os textos são próprios e não apenas placeholders;
- os links funcionam;
- o CSS fornecido não foi alterado.

## 5. Publicação, README e apresentação

Será avaliado se:

- o projeto está publicado com GitHub Pages;
- o link publicado está no `README.md`;
- o `README.md` descreve o projeto final;
- a apresentação mostra o site, Issues, Pull Requests e histórico;
- cada membro consegue explicar uma contribuição concreta.

---

# Apresentação final

Cada grupo faz uma demonstração curta, entre 3 e 5 minutos:

1. Abrir o projeto publicado.
2. Navegar pelas páginas.
3. Mostrar Issues e Pull Requests no GitHub.
4. Mostrar o histórico com:

```bash
git log --oneline --graph --all
```

---

# Checklist final

- [ ] Repositório GitHub chamado `projeto617`
- [ ] Branch principal chamada `main`
- [ ] `.gitignore` criado ou revisto pela equipa
- [ ] Todos os membros trabalharam no seu computador
- [ ] Todos atualizaram o `main` com `git pull` antes de criar branches
- [ ] Cada membro seguiu `tarefas/pagina-pessoal.md`
- [ ] Existe uma página pessoal por formando
- [ ] Cada página pessoal chama-se `membro-nome.html`
- [ ] Cada página pessoal foi criada a partir de `modelo.html`
- [ ] Cada página pessoal tem `h1`, parágrafos, listas e link de regresso
- [ ] Cada página pessoal tem pelo menos 7 secções com `class="cartao"`
- [ ] Cada página pessoal tem pelo menos 8 commits
- [ ] O menu do `index.html` liga todas as páginas
- [ ] O `index.html` foi construído em três sessões
- [ ] O `index.html` tem pelo menos 8 commits
- [ ] O `index.html` tem secções sobre equipa, método de trabalho, objetivo, membros, páginas, aprendizagens e próximos passos
- [ ] Cada página pessoal foi construída com várias etapas no mesmo branch
- [ ] As sessões do `index.html` foram feitas por ordem
- [ ] Houve um momento com vários Pull Requests abertos em paralelo
- [ ] O CSS fornecido não foi alterado
- [ ] Houve pelo menos um conflito real resolvido pela equipa
- [ ] Ninguém fez merge do seu próprio Pull Request
- [ ] Issues foram usadas para organizar o trabalho
- [ ] README final atualizado em branch próprio
- [ ] Projeto publicado com GitHub Pages
- [ ] Link do projeto publicado no README
- [ ] Apresentação final realizada

---

# Referência rápida de comandos

Esta secção serve apenas como apoio. A equipa deve escolher os comandos adequados a cada situação.

Atualizar o `main` antes de criar um branch novo:

```bash
git switch main
git pull
```

Criar branch:

```bash
git switch -c nome-do-branch
```

Ver alterações:

```bash
git status
git diff
```

Guardar alterações:

```bash
git add nome-do-ficheiro.html
git commit -m "Mensagem clara em português"
```

Enviar branch para GitHub:

```bash
git push -u origin nome-do-branch
```

Atualizar um branch com o `main`:

```bash
git switch nome-do-branch
git pull origin main
```

Ver histórico:

```bash
git log --oneline --graph --all
```
