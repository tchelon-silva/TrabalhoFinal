# Setup inicial do projeto617

Este guia é feito antes das páginas HTML.

Há dois papéis:

- **Owner do repositório**: cria/publica o repositório no GitHub e adiciona os colegas.
- **Restantes membros**: aceitam o convite e clonam o repositório.

O repositório deve chamar-se:

```text
projeto617
```

---

## Antes de começar

O owner usa a pasta starter fornecida pelo formador.

Antes de publicar, confirmar que a pasta contém, no mínimo:

```text
index.html
modelo.html
css/style.css
tarefas/
README.md
enunciado.md
```

O ficheiro `.gitignore` também deve existir antes do primeiro commit. Se ainda não existir, deve ser criado pela equipa.

---

## Parte A — Owner do repositório

O owner escolhe **uma** das opções seguintes:

- VS Code
- GitHub Desktop

Não há obrigação de usar o terminal para criar o repositório inicial. A ferramenta escolhida deve permitir:

1. inicializar Git na pasta do projeto;
2. criar o primeiro commit;
3. publicar o repositório no GitHub;
4. confirmar que a branch principal se chama `main`;
5. adicionar os colegas como colaboradores.

---

## Passo 1 — Criar ou confirmar o `.gitignore`

Antes do primeiro commit, a equipa deve confirmar o ficheiro `.gitignore`.

O `.gitignore` serve para indicar ficheiros e pastas que **não devem entrar no repositório**.

Exemplos de entradas que podem fazer sentido:

```gitignore
rascunhos/
*.tmp
Thumbs.db
.DS_Store
```

A decisão final fica ao critério da equipa. Devem pensar em ficheiros que:

- são temporários;
- são criados automaticamente pelo sistema operativo;
- são rascunhos pessoais;
- não fazem parte da entrega final.

Não devem colocar no `.gitignore` ficheiros necessários ao projeto, como:

- `index.html`
- `modelo.html`
- `css/style.css`
- `README.md`
- `enunciado.md`
- ficheiros da pasta `tarefas/`

Depois de criar ou rever o `.gitignore`, guardar o ficheiro.

---

## Passo 2 — Criar o repositório local

O owner cria o repositório Git local usando VS Code ou GitHub Desktop.

### Opção A — VS Code

No VS Code, usar a área **Source Control** para inicializar o repositório na pasta do projeto.

Depois, confirmar que o VS Code mostra os ficheiros alterados para o primeiro commit.

### Opção B — GitHub Desktop

No GitHub Desktop, adicionar a pasta do projeto como repositório local.

Depois, confirmar que a aplicação mostra os ficheiros alterados para o primeiro commit.

---

## Passo 3 — Garantir que a branch principal se chama `main`

Durante o curso, a branch principal usada será sempre:

```text
main
```

Algumas ferramentas podem criar a branch inicial com outro nome, por exemplo `master`.

Antes de publicar no GitHub, o owner deve confirmar o nome da branch.

Para verificar no terminal:

```bash
git branch
```

Se a branch aparecer como `master`, deve ser renomeada para `main` antes do primeiro push.

Uma forma de o fazer pelo terminal é:

```bash
git branch -M main
```

Função deste comando:

- `git branch` gere branches;
- `-M` renomeia a branch atual;
- `main` é o novo nome da branch.

Se estiverem a usar VS Code ou GitHub Desktop, também podem procurar a opção de renomear a branch na própria ferramenta.

O importante é: **antes de publicar, a branch principal deve chamar-se `main`**.

---

## Passo 4 — Criar o primeiro commit

O primeiro commit deve adicionar o starter do projeto.

Mensagem sugerida:

```text
Adiciona starter do projeto617
```

Antes de confirmar o commit, o owner deve verificar que entram no commit:

- ficheiros HTML iniciais;
- CSS fornecido;
- `README.md`;
- `enunciado.md`;
- guias da pasta `tarefas/`;
- `.gitignore`.

Não devem entrar ficheiros de rascunho, testes locais ou ficheiros temporários.

---

## Passo 5 — Publicar no GitHub

O owner publica o repositório no GitHub usando a ferramenta escolhida.

Nome obrigatório do repositório:

```text
projeto617
```

O repositório pode começar privado ou público, conforme indicação do formador.

Nota sobre GitHub Pages:

- Em contas GitHub Free, a publicação com GitHub Pages deve ser feita a partir de um repositório público.
- Se o repositório começar privado, a equipa deve confirmar com o formador quando o pode tornar público.

Depois de publicar, abrir o GitHub no browser e confirmar:

- o repositório chama-se `projeto617`;
- a branch principal chama-se `main`;
- os ficheiros do starter aparecem no GitHub;
- o primeiro commit tem uma mensagem clara.

---

## Passo 6 — Adicionar colaboradores

No GitHub, o owner adiciona os colegas como colaboradores do repositório `projeto617`.

Os colegas devem aceitar o convite antes de começarem a trabalhar.

---

## Parte B — Restantes membros

Cada membro trabalha no seu computador.

### Passo 1 — Aceitar convite

Cada membro aceita o convite para colaborar no repositório `projeto617`.

### Passo 2 — Clonar o repositório

Cada membro clona o repositório usando VS Code, GitHub Desktop ou outro método que conheça.

Não há um único caminho obrigatório. O formando deve conseguir:

- encontrar o repositório `projeto617` no GitHub;
- copiar ou usar o URL do repositório;
- escolher uma pasta local para guardar o projeto;
- abrir a pasta no editor;
- confirmar que os ficheiros aparecem localmente.

Se tiver dúvidas nos passos da ferramenta, deve consultar a documentação da ferramenta escolhida ou pedir validação ao formador.

### Passo 3 — Confirmar que está tudo certo

No fim do clone, cada membro confirma:

- a pasta local tem os ficheiros do starter;
- o repositório remoto é o `projeto617`;
- a branch principal é `main`;
- não existem alterações locais por guardar.

Comandos úteis para confirmar, se estiverem a usar terminal:

```bash
git status
git branch
git log --oneline
```

O histórico deve mostrar o commit inicial do starter.

---

## Resultado esperado

No fim deste setup:

- O repositório `projeto617` existe no GitHub.
- A branch principal chama-se `main`.
- O `.gitignore` foi criado ou revisto pela equipa.
- Todos os membros têm acesso ao repositório.
- Cada membro tem uma cópia local do projeto.
- Todos conseguem confirmar o estado do repositório antes de começar a trabalhar.
