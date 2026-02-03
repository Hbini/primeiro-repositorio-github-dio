# 📚 Exercício 1: Comandos Essenciais do Git

## Configuração Inicial do Git

### 1. Configurar Usuário e Email
```bash
git config --global user.name "Seu Nome"
git config --global user.email "seu.email@example.com"
```

### 2. Verificar Configurações
```bash
git config --list
```

## Criando e Clonando Repositórios

### 3. Inicializar um Repositório
```bash
git init meu-projeto
cd meu-projeto
```

### 4. Clonar um Repositório Existente
```bash
git clone https://github.com/usuario/repositorio.git
```

## Trabalhando com Commits

### 5. Verificar Status
```bash
git status
```

### 6. Adicionar Arquivos
```bash
# Adicionar arquivo específico
git add arquivo.txt

# Adicionar todos os arquivos
git add .

# Adicionar com patch (interativo)
git add -p
```

### 7. Criar um Commit
```bash
# Commit simples
git commit -m "Descrição da mudança"

# Commit com descrição detalhada
git commit -m "Título" -m "Descrição detalhada das mudanças"

# Commit com alterações de arquivos rastreados
git commit -am "Descrição"
```

### 8. Ver Histórico de Commits
```bash
# Histórico simples
git log

# Histórico com um commit por linha
git log --oneline

# Histórico gráfico de branches
git log --graph --oneline --all

# Ver mudanças de um arquivo específico
git log -- arquivo.txt
```

## Trabalhando com Branches

### 9. Criar e Mudar de Branch
```bash
# Listar branches locais
git branch

# Listar todas as branches
git branch -a

# Criar nova branch
git branch nome-branch

# Mudar para uma branch
git checkout nome-branch

# Criar e mudar simultaneamente
git checkout -b nome-branch
```

### 10. Merge de Branches
```bash
# Fazer merge de uma branch na atual
git merge nome-branch

# Merge com mensagem customizada
git merge nome-branch -m "Mensagem"
```

## Desfazendo Mudanças

### 11. Descartar Mudanças
```bash
# Descartar mudanças em arquivo
git checkout -- arquivo.txt

# Descartar todas as mudanças
git reset --hard HEAD
```

### 12. Desfazer Último Commit
```bash
# Desfazer commit mas manter mudanças
git reset --soft HEAD~1

# Desfazer commit e descartar mudanças
git reset --hard HEAD~1
```

## Sincronizando com Remoto

### 13. Trabalhar com Remoto
```bash
# Ver repositórios remotos
git remote -v

# Adicionar repositório remoto
git remote add origin https://github.com/usuario/repo.git

# Fazer pull (fetch + merge)
git pull origin main

# Fazer push
git push origin main

# Push de nova branch
git push -u origin nome-branch
```

## Exercício Prático

1. Crie um novo repositório local
2. Configure seu usuário do Git
3. Crie um arquivo README.md
4. Faça um commit
5. Crie uma nova branch "feature"
6. Faça mudanças e commit
7. Volte para main e faça merge
8. Verifique o histórico com log --graph

Parabéns! Você completou o exercício dos comandos essenciais do Git! 🎉
