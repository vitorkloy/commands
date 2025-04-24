# commands

### 📦 **1. Inicializar o repositório**
```bash
git init
```
Cria um novo repositório Git na pasta atual.

---

### 📁 **2. Clonar um repositório existente (do GitHub, por exemplo)**
```bash
git clone https://github.com/usuario/repositorio.git
```
Copia o repositório remoto para sua máquina.

---

### ✅ **3. Verificar o status dos arquivos**
```bash
git status
```
Mostra os arquivos modificados e prontos para serem adicionados/commitados.

---

### ➕ **4. Adicionar arquivos para serem commitados**
```bash
git add nome-do-arquivo
# ou para todos os arquivos:
git add .
```
Coloca os arquivos na "área de preparação" (stage).

---

### 💾 **5. Salvar as alterações com uma mensagem**
```bash
git commit -m "mensagem explicando o que foi feito"
```
Grava as mudanças no histórico do Git.

---

### 🔗 **6. Conectar ao repositório do GitHub**
```bash
git remote add origin https://github.com/usuario/repositorio.git
```
Conecta o repositório local com o remoto no GitHub.

---

### 📤 **7. Enviar o projeto para o GitHub**
```bash
git push -u origin main
```
Envia os commits para o GitHub (geralmente o nome do branch principal é `main`, mas pode ser `master` em repositórios antigos).

---

### 🔄 **8. Puxar alterações do GitHub**
```bash
git pull origin main
```
Baixa alterações feitas no repositório remoto.

---

### 🌳 **9. Criar uma nova branch**
```bash
git checkout -b nome-da-branch
```
Cria e muda para uma nova branch.

---

### 🔁 **10. Juntar uma branch com a main**
```bash
git checkout main
git merge nome-da-branch
```
Aplica as alterações da branch na branch principal.

