<div class="header">
  <h1>git</h1>
  <img height="40" width="250" src="assets/sie-logo-collection-v2-1-0/Online/PNG/sie-logo-petrol-rgb.png" alt="Logo Siemens">
</div>

<!-- # Material de Acompanhamento para Treinamento de Git

---

## 📖 Sumário

- [Introdução ao Git e sua Importância](#introdução-ao-git-e-sua-importância)
- [Configuração do Ambiente](#configuração-do-ambiente)
  - [Instalação](#instalação)
  - [Configurações Iniciais](#configurações-iniciais)
- [Comandos Essenciais e Exemplos Práticos](#comandos-essenciais-e-exemplos-práticos)
  - [`git init`](#git-init)
  - [`git clone`](#git-clone)
  - [`git add`](#git-add)
  - [`git commit`](#git-commit)
  - [`git status`](#git-status)
  - [`git log`](#git-log)
- [Gerenciamento de Branches](#gerenciamento-de-branches)
  - [Criando e alternando branches](#criando-e-alternando-branches)
  - [Merge entre branches](#merge-entre-branches)
  - [Resolução de conflitos](#resolução-de-conflitos)
- [Fluxo de Trabalho Colaborativo](#fluxo-de-trabalho-colaborativo)
  - [`git pull`](#git-pull)
  - [`git push`](#git-push)
  - [Fork e Pull Request](#fork-e-pull-request)
- [Boas Práticas e Dicas Úteis](#boas-práticas-e-dicas-úteis)
- [Prós e Contras](#prós-e-contras)
- [Conclusão](#conclusão)

--- -->

## 📝 Introdução ao Git e sua Importância

Git é um sistema de controle de versão distribuído amplamente utilizado, criado por Linus Torvalds. Tem como principal objetivo controlar versões de código-fonte e facilitar o trabalho colaborativo em projetos de software.

**Importância do Git:**

- Histórico consistente das alterações.
- Facilita o trabalho colaborativo.
- Segurança e backup dos arquivos.
- Simplifica a resolução de conflitos.

---

## ⚙️ Configuração do Ambiente

### Instalação

Siga as instruções para instalar o Git de acordo com o seu sistema operacional: [Download Git](https://git-scm.com/downloads).

### Configurações Iniciais

Configure as informações básicas após instalação:

```bash
git config --global user.name "Seu Nome"
git config --global user.email "seuemail@exemplo.com"
git config --global core.editor seu_editor
git config --global init.defaultBranch main
```

---

<div style="page-break-after: always;"></div>

## 🚀 Comandos Essenciais e Exemplos Práticos

### `git init`

Cria um novo repositório Git em um diretório existente.

```bash
git init nome-projeto
```

### `git clone`

Cria uma cópia local de um repositório remoto existente.

```bash
git clone https://github.com/seu-usuario/nome-repositorio.git
```

### `git add`

Adiciona arquivos para serem rastreados pelo Git.

```bash
git add arquivo.txt
git add .
```

### `git commit`

Grava as alterações no repositório local.

```bash
git commit -m "Breve mensagem descritiva"
```

### `git status`

Exibe o estado atual do diretório de trabalho e staging.

```bash
git status
```

### `git log`

Mostra histórico detalhado dos commits.

```bash
git log
git log --oneline
```

---

<div style="page-break-after: always;"></div>

## 🌳 Gerenciamento de Branches

### Criando e alternando branches

Criação e troca entre branches.

```bash
git branch nova-branch
git checkout nova-branch

#alternativa direta de criar e trocar ao mesmo tempo:
git checkout -b nova-branch
```

### Merge entre branches

Une alterações de branches diferentes.

```bash
git checkout main
git merge nome-da-branch
```

### Resolução de conflitos

Quando o Git não consegue resolver automaticamente conflitos:

1. Verifique os arquivos com conflito:

```bash
git status
```

2. Resolva conflitos manualmente no editor.
3. Após resolver:

```bash
git add arquivo-resolvido.txt
git commit -m "Resolve conflito de merge"
```

---

<div style="page-break-after: always;"></div>

## 🤝 Fluxo de Trabalho Colaborativo

### `git pull`

Busca atualizações do repositório remoto para o local.

```bash
git pull origin main
```

### `git push`

Envia alterações locais para um repositório remoto.

```bash
git push origin nome-da-branch
```

### Fork e Pull Request

- **Fork:** cria uma cópia do repositório original para o seu GitHub.
- **Pull Request (PR):** Solicitação para unir suas alterações com o repositório original.

Fluxo:

1. Faça fork do repositório no GitHub.
2. Clone o repositório que foi copiado para seu GitHub.
3. Crie e altere branches localmente.
4. Envie alterações para seu repositório remoto.
5. Abra um Pull Request no repositório original.

---

## 💡 Boas Práticas e Dicas Úteis

- Commits pequenos e frequentes.
- Mensagens de commit significativas.
- Uso consistente de branches.
- Evite conflitos: sempre faça pull antes de começar a editar.
- Utilize `.gitignore` para arquivos sensíveis ou desnecessários.

---

<div style="page-break-after: always;"></div>

## ⚖️ Prós e Contras

### ✅ Prós:

- Fácil colaboração em projetos.
- Gestão eficiente das versões.
- Histórico completo de alterações.
- Interface potente e flexível via linha de comando.

### ❌ Contras:

- Curva de aprendizado inicial pode ser acentuada.
- Reposição de dados apagados ou alterados por acidente pode ser complexa.
- Conflitos frequentes em projetos grandes e equipes mal orientadas.

---

## 🎯 Conclusão

Git é uma poderosa ferramenta que ajuda equipes a trabalharem juntas com organização e produtividade. Dominar seu uso otimiza fluxos de trabalho e garante confiabilidade ao controle das versões. Continue praticando consistentemente e explore recursos avançados e melhores práticas para tirar o máximo proveito do Git.

---
