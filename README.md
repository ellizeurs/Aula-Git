# Repositório de Aula de Git

Este repositório contém material de apoio para aulas de Git, incluindo:

- Exercício básico de Git com terminal e Vim
- Slides em PDF explicando comandos e conceitos
- Pasta `alunos/` para prática de Pull Requests com workflow automático

---

## 📁 Conteúdo

### 1. Exercício Básico de Git
- Localização: [`exercício/README.md`](exercício/README.md)
- Inclui:
  - Inicialização de repositório (`git init`)
  - Commits (`git add` / `git commit`)
  - Criação e troca de branches
  - Visualização de status e logs (`git status`, `git log`)
  - Configuração de remoto SSH e push para GitHub

### 2. Slides em PDF
- Localização: [`slides/introducao_git.pdf`](slides/introducao_git.pdf)
- Contém:
  - Resumo de comandos (`init`, `status`, `log`, `branch`, `checkout/switch`, `merge`, `push`)
  - Branches no Git Flow (`main`, `develop`, `feature`, `release`, `hotfix`)
  - Uso de issues e workflow básico
  - Exemplos visuais e passo a passo para aula

### 3. Pasta `alunos/`
- Localização: [`alunos/`](alunos/)
- Destinada a cada aluno criar seu próprio arquivo Markdown (`{username}.md`) e se apresentar.
- **Instruções para os alunos**:
  1. Faça **fork** deste repositório.
  2. Crie ou atualize seu arquivo dentro da pasta:
     ```
     alunos/{seu-username}.md
     ```
  3. No arquivo, escreva uma breve apresentação (nome, curso, interesses etc.).
  4. Abra um **Pull Request** para o branch `main` deste repositório.
- **Workflow automático**:
  - PRs são validados para garantir que apenas o arquivo correspondente ao seu nome de usuário seja modificado.
  - Se passar a validação, o PR é **mergeado automaticamente**.
  - Se falhar, o PR é bloqueado e recebe um comentário explicando o motivo.

---

## 📌 Observações

- Este repositório é destinado a prática em aula.  
- Recomenda-se criar o repositório local e configurar o SSH antes de iniciar o exercício.  
- O PDF dos slides pode ser usado como guia durante a aula.  
- Para a pasta `alunos/`, cada aluno deve manter apenas o seu próprio arquivo e seguir o workflow descrito.
