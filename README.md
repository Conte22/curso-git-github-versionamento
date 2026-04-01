# 📘 Curso Git & GitHub — Versionamento na Prática

  Este repositório foi criado como exercício prático de versionamento com **Git** e **GitHub**.
  Ele contém exemplos de commits e serve como referência de estudo.

  ---

  ## 🧠 O que é Git?

  **Git** é um sistema de controle de versão distribuído. Ele registra as alterações feitas em arquivos ao longo do tempo, permitindo que você:

  - Volte a versões anteriores do projeto
  - Trabalhe em equipe sem sobrescrever o trabalho uns dos outros
  - Crie ramificações (branches) para testar novas funcionalidades

  ---

  ## 🌐 O que é GitHub?

  **GitHub** é uma plataforma web que hospeda repositórios Git na nuvem. Com ele, você pode:

  - Publicar seu código online
  - Colaborar com outras pessoas
  - Acompanhar o histórico de mudanças

  ---

  ## ⚙️ Configuração inicial (apenas uma vez)

  Antes de começar, configure seu nome e e-mail no Git:

  ```bash
  git config --global user.name "Seu Nome"
  git config --global user.email "seu@email.com"
  ```

  ---

  ## 🚀 Como criar um repositório local e conectar ao GitHub

  ```bash
  # 1. Inicialize o Git na pasta do projeto
  git init

  # 2. Conecte ao repositório remoto no GitHub
  git remote add origin https://github.com/SEU_USUARIO/SEU_REPOSITORIO.git

  # 3. Defina a branch principal como 'main'
  git branch -M main
  ```

  ---

  ## 📝 Como realizar commits e enviar ao repositório

  ### Passo a passo completo:

  ```bash
  # 1. Verifique o status dos arquivos (quais foram modificados)
  git status

  # 2. Adicione os arquivos ao "stage" (área de preparação)
  git add nome-do-arquivo.txt     # Adiciona um arquivo específico
  git add .                        # Adiciona todos os arquivos modificados

  # 3. Crie um commit com uma mensagem descritiva
  git commit -m "feat: descrição clara do que foi feito"

  # 4. Envie o commit para o GitHub (repositório remoto)
  git push origin main
  ```

  ---

  ## 🔄 Fluxo típico de trabalho

  ```text
  Editar arquivo(s)
         ↓
  git add .
         ↓
  git commit -m "mensagem"
         ↓
  git push origin main
  ```

  ---

  ## 💡 Boas práticas para mensagens de commit

  Use mensagens claras e no formato:

  | Prefixo     | Quando usar                          |
  |-------------|--------------------------------------|
  | `feat:`     | Nova funcionalidade                  |
  | `fix:`      | Correção de bug                      |
  | `docs:`     | Alteração em documentação            |
  | `style:`    | Formatação, sem mudança de lógica    |
  | `refactor:` | Refatoração de código                |
  | `chore:`    | Tarefas de manutenção                |

  **Exemplos:**
  ```bash
  git commit -m "feat: adiciona sistema de login"
  git commit -m "fix: corrige erro no cálculo de total"
  git commit -m "docs: atualiza README com instruções de instalação"
  ```

  ---

  ## 📋 Comandos úteis

  ```bash
  git log --oneline        # Ver histórico resumido de commits
  git diff                 # Ver o que mudou antes de fazer o commit
  git pull origin main     # Baixar atualizações do repositório remoto
  git clone URL            # Clonar um repositório existente
  ```

  ---

  ## 📁 Estrutura deste repositório

  ```
  curso-git-github-versionamento/
  ├── README.md          # Documentação principal (este arquivo)
  ├── notas.txt          # Anotações do curso
  └── aprendizados.md    # Resumo dos principais aprendizados
  ```

  ---

  > Criado como parte do exercício de versionamento do curso de Git e GitHub.
  