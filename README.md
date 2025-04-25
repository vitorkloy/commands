# Git Commands Guide 🚀

Comandos essenciais do Git e soluções para erros comuns que podem aparecer ao fazer `commit` ou outras operações:

#### Este README inclui:
1. Todos os comandos básicos
2. Fluxo de trabalho com branches
3. Soluções para erros comuns (especialmente relacionados a commit/push)
4. Comandos úteis para histórico e configuração
5. Dicas para evitar problemas
   
---

## 🔧 **Comandos Básicos**

### 📦 **1. Inicializar um repositório**
```bash
git init
```

### 📁 **2. Clonar um repositório**
```bash
git clone https://github.com/usuario/repositorio.git
```

### ✅ **3. Verificar status**
```bash
git status
```

### ➕ **4. Adicionar arquivos**
```bash
git add nome-do-arquivo  # Arquivo específico
git add .                # Todos os arquivos
git add -A               # Todos os arquivos (incluindo deletados)
```

### 💾 **5. Fazer commit**
```bash
git commit -m "mensagem descritiva"
```

### 🔗 **6. Conectar ao repositório remoto**
```bash
git remote add origin https://github.com/usuario/repositorio.git
```

### 📤 **7. Enviar para o repositório remoto**
```bash
git push -u origin main  # Primeiro push
git push                 # Pushes seguintes
```

### 🔄 **8. Atualizar do repositório remoto**
```bash
git pull origin main
```

---

## 🌿 **Branching & Merging**

### 🌳 **9. Criar e mudar para nova branch**
```bash
git checkout -b nome-da-branch
```

### 🔀 **10. Alternar entre branches**
```bash
git checkout nome-da-branch
```

### 🔁 **11. Merge (juntar branches)**
```bash
git checkout main
git merge nome-da-branch
```

### 🗑️ **12. Deletar branch**
```bash
git branch -d nome-da-branch      # Deleta local
git push origin --delete nome-da-branch  # Deleta remoto
```

---

## ⚠️ **Soluções para Erros Comuns**

### 🔄 **Erro ao fazer push (divergência de branches)**
```bash
git pull --rebase origin main
git push origin main
```

### ✏️ **Corrigir último commit (mensagem ou arquivos)**
```bash
git add .                        # Adiciona arquivos esquecidos
git commit --amend -m "nova mensagem"
git push --force origin main     # Cuidado: força push
```

### 🔍 **Desfazer commit local (mantendo alterações)**
```bash
git reset --soft HEAD~1
```

### ⏪ **Desfazer commit local (perdendo alterações)**
```bash
git reset --hard HEAD~1
```

### 🗄️ **Recuperar arquivos deletados**
```bash
git checkout HEAD -- nome-do-arquivo
```

### 🔀 **Resolver conflitos de merge**
1. Abra os arquivos com conflitos (<<<<<<< HEAD)
2. Edite para manter as versões corretas
3. Depois de resolver:
```bash
git add .
git commit -m "resolve merge conflicts"
```

---

## 📜 **Histórico & Logs**

### 📋 **Ver histórico de commits**
```bash
git log
git log --oneline          # Versão compacta
git log --graph --oneline  # Com visualização de branches
```

### 🔎 **Buscar alterações em arquivos**
```bash
git blame nome-do-arquivo  # Mostra quem editou cada linha
```

---

## 🧠 **Comandos Avançados Úteis**

### 🕵️ **Encontrar bugs**
```bash
git bisect start                    # Inicia busca binária
git bisect bad                      # Marca commit atual como ruim
git bisect good <hash-old-commit>   # Marca commit antigo como bom
```

### 🏷️ **Versionamento**
```bash
git tag -a v1.0.0 -m "Versão estável"
git push origin v1.0.0
```

### 🗂️ **Reescrever histórico (cuidado!)**
```bash
git rebase -i HEAD~3  # Edita últimos 3 commits
```

---

## ⚙️ **Configurações Úteis**

### 👤 **Configurar usuário**
```bash
git config --global user.name "Seu Nome"
git config --global user.email "seu@email.com"
```

### 🔑 **Salvar credenciais (evitar pedir senha sempre)**
```bash
git config --global credential.helper store
```

### 🛠️ **Ignorar arquivos (`.gitignore`)**
Crie um arquivo `.gitignore` na raiz do projeto com:
```
node_modules/
.env
*.log
```

---

💡 **Dica**: Sempre verifique `git status` antes e depois de operações para entender o estado do seu repositório!
