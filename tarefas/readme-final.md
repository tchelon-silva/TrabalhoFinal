# README final

Esta tarefa é feita no fim do projeto, depois de:

- as páginas pessoais estarem no `main`;
- o `index.html` estar terminado;
- o conflito do lema estar resolvido;
- o projeto estar publicado com GitHub Pages.

---

## Objetivo desta etapa

Atualizar o `README.md` inicial para passar a ser a documentação final do projeto.

O `README.md` é a primeira página que aparece quando alguém abre o repositório no GitHub. Deve explicar, de forma clara, o que foi feito, quem participou e como o trabalho foi organizado.

A equipa **não cria outro README**. Atualiza o ficheiro `README.md` que já existe no starter.

---

## Estrutura do `README.md`

O `README.md` final deve ter as seguintes secções.

### 1. Título

Identifica o projeto.

Conteúdo esperado:

- nome do projeto: `projeto617`.

### 2. Projeto publicado

Indica onde o site pode ser visto online.

Conteúdo esperado:

- link do GitHub Pages;
- o link deve abrir corretamente no browser.

### 3. Descrição

Explica o projeto em poucas frases.

Conteúdo esperado:

- indicar que é um projeto de grupo da UC00617;
- indicar que é um pequeno site em HTML;
- explicar que o foco foi praticar Git, GitHub, branches, commits, Pull Requests e conflitos.

### 4. Equipa

Identifica os membros do grupo.

Conteúdo esperado:

- nome de cada formando;
- não usar nomes genéricos como Ana, Bruno ou Carla, exceto se forem os nomes reais do grupo.

### 5. Páginas

Lista as páginas existentes no projeto.

Conteúdo esperado:

- `index.html`;
- uma página pessoal por membro;
- breve descrição de cada página.

### 6. Trabalho realizado

Resume o que a equipa fez.

Conteúdo esperado:

- criação das páginas pessoais;
- construção conjunta do `index.html`;
- uso de branches;
- uso de commits;
- abertura e revisão de Pull Requests;
- resolução do conflito do lema.

### 7. Tecnologias usadas

Lista as tecnologias e ferramentas utilizadas.

Conteúdo esperado:

- HTML;
- CSS fornecido pelo formador;
- Git;
- GitHub;
- GitHub Pages.

### 8. Organização do trabalho

Explica como a equipa colaborou.

Conteúdo esperado:

- cada página pessoal foi feita num branch próprio;
- o `index.html` foi feito em sessões;
- os Pull Requests foram revistos por colegas;
- ninguém fez merge do seu próprio Pull Request;
- o conflito obrigatório foi resolvido antes da entrega.

## Forma de trabalho

Esta tarefa deve ser feita num branch próprio.

Nome sugerido para o branch:

```text
docs/readme-final
```

O trabalho deve ser dividido em pelo menos 3 commits.

Sugestão de divisão:

1. atualizar título, link publicado e descrição;
2. adicionar equipa e páginas;
3. adicionar trabalho realizado, tecnologias e organização.

Esta divisão é uma orientação. A equipa pode organizar os commits de outra forma, desde que sejam claros e façam sentido.

### Etapa R1 — Título, link e descrição

Conteúdo a criar ou rever:

- título `projeto617`;
- link do projeto publicado;
- descrição curta do projeto.

Commit da etapa:

- criar um commit só com estas alterações;
- mensagem sugerida: `Atualiza titulo link e descricao do README`.

### Etapa R2 — Equipa e páginas

Conteúdo a criar:

- secção `Equipa`;
- lista dos membros reais do grupo;
- secção `Páginas`;
- lista das páginas criadas.

Commit da etapa:

- criar um commit só com estas secções;
- mensagem sugerida: `Documenta equipa e paginas no README`.

### Etapa R3 — Processo, tecnologias e organização

Conteúdo a criar:

- secção `Trabalho realizado`;
- secção `Tecnologias usadas`;
- secção `Organização do trabalho`.

Commit da etapa:

- criar um commit só com estas secções;
- mensagem sugerida: `Completa documentacao final do README`.

---

## Comandos de apoio

Os comandos não estão escritos em cada passo de propósito.

O formando deve escolher os comandos adequados ao momento de trabalho.

Comandos que podem ser necessários:

```bash
git switch main
git pull
git switch -c docs/readme-final
git status
git diff
git add README.md
git commit -m "Mensagem clara em portugues"
git push -u origin docs/readme-final
git log --oneline
```

A mensagem do commit deve ser decidida pelo formando, de acordo com a alteração feita.

---

## Revisão antes do Pull Request

Antes de abrir o Pull Request, confirmar:

- o ficheiro alterado é o `README.md`;
- o README tem todas as secções obrigatórias;
- o link do GitHub Pages funciona;
- os nomes dos membros estão corretos;
- os nomes das páginas correspondem aos ficheiros reais;
- não há texto temporário;
- existem pelo menos 3 commits no branch;
- o projeto continua organizado.

---

## Pull Request

Depois de terminar o README:

1. enviar o branch para o GitHub;
2. abrir um Pull Request;
3. usar um título claro;
4. resumir o que foi alterado;
5. pedir revisão a um colega;
6. garantir que o autor do Pull Request não faz merge do seu próprio trabalho.

Título sugerido:

```text
Atualiza README final
```

---

## Resultado final esperado

No fim desta tarefa:

- o `README.md` apresenta o projeto final;
- o link do projeto publicado está visível;
- a equipa está identificada;
- todas as páginas estão listadas;
- o processo de trabalho está explicado;
- as tecnologias usadas estão indicadas;
- a organização do trabalho está descrita;
- o Pull Request do README foi revisto e aceite por um colega.
