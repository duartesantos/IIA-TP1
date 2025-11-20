# Instruções para Criar o Repositório Git

## Inicializar o Repositório Local

1. Abra o terminal/PowerShell na pasta do projeto
2. Execute os seguintes comandos:

```bash
# Inicializar o repositório Git
git init

# Adicionar todos os ficheiros (exceto os ignorados pelo .gitignore)
git add .

# Fazer o primeiro commit
git commit -m "Initial commit: Trabalho Prático 1 - Simulação de Aspiradores Autônomos"
```

## Criar Repositório no GitHub/GitLab

### GitHub

1. Aceda a [GitHub](https://github.com) e faça login
2. Clique em "New repository" (ou "Novo repositório")
3. Preencha:
   - **Repository name**: `IIA-TP1-Aspiradores` (ou outro nome à sua escolha)
   - **Description**: "Trabalho Prático 1 - Simulação de Aspiradores Autônomos em NetLogo"
   - **Visibility**: Escolha entre Public ou Private
   - **NÃO** inicialize com README, .gitignore ou licença (já temos)
4. Clique em "Create repository"
5. Siga as instruções que aparecem no GitHub para ligar o repositório local:

```bash
# Adicionar o repositório remoto (substitua USERNAME pelo seu username)
git remote add origin https://github.com/USERNAME/IIA-TP1-Aspiradores.git

# Renomear a branch principal para main (se necessário)
git branch -M main

# Fazer push do código
git push -u origin main
```

### GitLab

1. Aceda a [GitLab](https://gitlab.com) e faça login
2. Clique em "New project" → "Create blank project"
3. Preencha:
   - **Project name**: `IIA-TP1-Aspiradores`
   - **Project slug**: Será gerado automaticamente
   - **Visibility Level**: Escolha entre Public ou Private
4. Clique em "Create project"
5. Siga as instruções que aparecem no GitLab:

```bash
# Adicionar o repositório remoto (substitua USERNAME pelo seu username)
git remote add origin https://gitlab.com/USERNAME/IIA-TP1-Aspiradores.git

# Renomear a branch principal para main (se necessário)
git branch -M main

# Fazer push do código
git push -u origin main
```

## Comandos Úteis

```bash
# Ver o estado do repositório
git status

# Ver o histórico de commits
git log

# Adicionar ficheiros específicos
git add nome_do_ficheiro

# Fazer commit com mensagem
git commit -m "Descrição das alterações"

# Fazer push das alterações
git push

# Ver branches
git branch

# Criar nova branch
git checkout -b nome-da-branch
```

## Estrutura Recomendada do Repositório

O repositório deve conter:
- ✅ `README.md` - Documentação principal
- ✅ `.gitignore` - Ficheiros a ignorar
- ✅ `tp1.nlogo` - Código fonte
- ✅ `IIA_2425_TP1.pdf` - Enunciado (se permitido)
- ✅ `DuarteSantos_2022149622_GustavoCosta_2023145800.pdf` - Relatório (se permitido)
- ❌ `desktop.ini` - Será ignorado pelo .gitignore
- ❌ Ficheiros temporários - Serão ignorados

## Notas Importantes

- Certifique-se de que os PDFs podem ser partilhados publicamente antes de fazer push
- Se os PDFs contiverem informações sensíveis, considere torná-los privados ou removê-los
- O ficheiro `.gitignore` já está configurado para ignorar ficheiros do sistema Windows

