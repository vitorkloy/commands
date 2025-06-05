# Git Commands Guide 🚀

Comandos do Git, organizados por categoria, para utilizar com o GitHub. Esta lista inclui comandos desde os mais básicos até os mais avançados, cobrindo diversas funcionalidades do Git.

---

## 🛠️ Configuração Inicial

* `git config --global user.name "Seu Nome"`: Define o nome do usuário.
* `git config --global user.email "seu@email.com"`: Define o e-mail do usuário.
* `git config --global core.editor "nome_do_editor"`: Define o editor padrão (por exemplo, `vim`, `nano`).
* `git config --list`: Lista todas as configurações atuais.

---

## 📁 Iniciando e Clonando Repositórios

* `git init`: Inicializa um novo repositório Git local.
* `git clone https://github.com/usuario/repositorio.git`: Clona um repositório remoto existente.

---

## 📄 Trabalhando com Arquivos

* `git status`: Mostra o status dos arquivos no diretório de trabalho e na área de stage.
* `git add arquivo.txt`: Adiciona um arquivo específico à área de stage.
* `git add .`: Adiciona todos os arquivos modificados à área de stage.
* `git commit -m "Mensagem do commit"`: Salva as alterações adicionadas com uma mensagem descritiva.
* `git commit --amend`: Modifica o último commit.
* `git rm arquivo.txt`: Remove um arquivo do repositório e do sistema de arquivos.
* `git mv arquivo_antigo.txt novo_arquivo.txt`: Renomeia ou move um arquivo.([atlassian.com][1])

---

## 🔄 Sincronização com Repositórios Remotos

* `git remote add origin https://github.com/usuario/repositorio.git`: Adiciona um repositório remoto.
* `git push -u origin main`: Envia as alterações para o repositório remoto na branch principal.
* `git pull origin main`: Atualiza o repositório local com as alterações do remoto.
* `git fetch`: Baixa as alterações do repositório remoto sem mesclá-las automaticamente.

---

## 🌿 Gerenciamento de Branches

* `git branch`: Lista todas as branches locais.
* `git branch nome-da-branch`: Cria uma nova branch.
* `git checkout nome-da-branch`: Muda para a branch especificada.
* `git checkout -b nova-branch`: Cria e muda para uma nova branch.
* `git merge nome-da-branch`: Mescla a branch especificada na branch atual.
* `git branch -d nome-da-branch`: Exclui uma branch local.
* `git push origin --delete nome-da-branch`: Exclui uma branch no repositório remoto.([loginradius.com][2], [github.com][3])

---

## 🕵️‍♂️ Visualização e Histórico

* `git log`: Exibe o histórico de commits.
* `git log --oneline`: Exibe o histórico de commits em uma linha por commit.
* `git diff`: Mostra as diferenças entre os arquivos modificados e o último commit.
* `git show`: Mostra detalhes sobre um objeto Git (como um commit).([education.github.com][4])

---

## 🧪 Stash e Recuperação de Alterações

* `git stash`: Salva temporariamente as alterações não commitadas.
* `git stash list`: Lista os stashes salvos.
* `git stash apply`: Aplica o último stash salvo.
* `git stash drop`: Remove o último stash salvo.
* `git stash clear`: Remove todos os stashes salvos.

---

## 🧹 Limpeza e Reset

* `git clean -f`: Remove arquivos não rastreados do diretório de trabalho.
* `git reset arquivo.txt`: Remove um arquivo da área de stage.
* `git reset --soft HEAD~1`: Desfaz o último commit, mantendo as alterações na área de stage.
* `git reset --hard HEAD~1`: Desfaz o último commit e descarta as alterações.

---

## 🏷️ Tags

* `git tag`: Lista todas as tags.
* `git tag -a v1.0 -m "Versão 1.0"`: Cria uma tag anotada.
* `git push origin v1.0`: Envia a tag para o repositório remoto.
* `git tag -d v1.0`: Exclui uma tag local.
* `git push origin --delete v1.0`: Exclui uma tag no repositório remoto.([github.com][3])

---

## 🔍 Outras Ferramentas Úteis

* `git blame arquivo.txt`: Mostra quem modificou cada linha de um arquivo.
* `git reflog`: Exibe o histórico de referências (como mudanças de HEAD).
* `git cherry-pick hash_do_commit`: Aplica um commit específico em outra branch.
* `git bisect`: Auxilia na identificação de commits que introduziram bugs.([atlassian.com][1], [learn.microsoft.com][5])

---

## 📚 Recursos Adicionais

* [Documentação Oficial do Git](https://git-scm.com/docs)
* [GitHub Education - Git Cheat Sheet (PDF)](https://education.github.com/git-cheat-sheet-education.pdf)
* [Git Reference](https://git.github.io/git-reference/)
