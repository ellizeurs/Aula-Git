# Exercício Básico de Git

Este exercício cobre os comandos básicos de Git, incluindo:

- Inicializar repositório (`git init`)
- Criar commits (`git add` / `git commit`)
- Criar e alternar branches
- Visualizar status e histórico (`git status`, `git log`)
- Adicionar repositório remoto e enviar para GitHub
- Configurar SSH para autenticação

---

## 1) Preparação: Gerar chave SSH e configurar GitHub

1. Gere uma chave SSH (se ainda não tiver):
```bash
ssh-keygen -t ed25519 -C "seu@email.com"
````

* Pressione `Enter` para aceitar o local padrão.
* Opcional: defina uma senha para a chave.

2. Copie a chave pública:

`````bash
cat ~/.ssh/id_ed25519.pub
`````

3. No GitHub: vá em **Settings → SSH and GPG keys → New SSH key** e cole a chave pública.

4. Configure Git com seu nome e email:

`````bash
git config --global user.name "Seu Nome"
git config --global user.email "seu@email.com"
`````

---

## 2) Criar repositório local

`````bash
mkdir git-basico
cd git-basico
git init -b main
`````

---

## 3) Criar e editar arquivo

`````bash
vim README.md
`````

No Vim, pressione `i` e adicione:

`````
# Repositório Básico
Exercício de Git básico.
`````

Salvar e sair: `Esc` → `:wq`

---

## 4) Verificar status e fazer commit

`````bash
git status
git add README.md
git commit -m "Adiciona README inicial"
`````

---

## 5) Criar e alternar para uma branch de teste

`````bash
git branch teste
git switch teste
`````

Edite ou crie outro arquivo:

`````bash
vim teste.txt
`````

Adicionar e commitar:

`````bash
git add teste.txt
git commit -m "Adiciona arquivo de teste"
`````

---

## 6) Voltar para a branch principal e mesclar

`````bash
git switch main
git merge teste
`````

---

## 7) Verificar log e status

`````bash
git status
git log --oneline --graph --all
`````

---

## 8) Adicionar repositório remoto e enviar

1. Crie um repositório vazio no GitHub chamado `git-basico`.
2. Adicione o remoto via SSH e envie:

`````bash
git remote add origin git@github.com:SEU_USUARIO/git-basico.git
git push -u origin main
`````

---

### ✅ Resultado esperado

* Repositório local com branch `main` e `teste`.
* Commits iniciais e de teste criados.
* Histórico visível com `git log`.
* Repositório remoto configurado via SSH com conteúdo enviado.
