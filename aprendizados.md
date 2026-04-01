# Principais Aprendizados — Git e GitHub

  ## O que é versionamento de código?

  Versionamento é o processo de **registrar e gerenciar mudanças** em arquivos ao longo do tempo.
  Com Git, cada mudança fica salva em um "commit", criando um histórico completo do projeto.

  ---

  ## Por que usar Git?

  | Sem Git                              | Com Git                                |
  |--------------------------------------|----------------------------------------|
  | Arquivos como "versao_final2.txt"    | Histórico organizado de mudanças       |
  | Impossível colaborar sem conflitos   | Colaboração estruturada em equipe      |
  | Sem como voltar atrás com segurança  | Fácil reversão para qualquer versão    |
  | Código perdido se o HD falhar        | Backup na nuvem via GitHub             |

  ---

  ## Os 3 conceitos mais importantes

  ### 1. Commit
  Um commit é um **snapshot (foto)** do projeto em determinado momento.
  Cada commit tem:
  - Uma mensagem descritiva
  - Um identificador único (SHA hash)
  - Referência ao commit anterior (exceto o primeiro)

  ### 2. Branch (Ramificação)
  Uma branch é uma **linha independente de desenvolvimento**.
  - A branch principal geralmente se chama `main`
  - Crie branches para novas funcionalidades sem afetar o código estável
  - Ao terminar, faça o merge de volta para a `main`

  ### 3. Remote (Repositório Remoto)
  O remote é a **cópia do repositório na nuvem** (ex: GitHub).
  - `git push`: envia seus commits locais para o GitHub
  - `git pull`: baixa commits do GitHub para sua máquina

  ---

  ## Meu fluxo de trabalho aprendido

  ```bash
  # 1. Clonar o projeto (apenas na primeira vez)
  git clone https://github.com/usuario/repositorio.git

  # 2. Trabalhar e modificar arquivos normalmente...

  # 3. Ver o que mudou
  git status
  git diff

  # 4. Preparar as mudanças para o commit
  git add .

  # 5. Criar o commit
  git commit -m "tipo: o que foi feito de forma clara e objetiva"

  # 6. Enviar para o GitHub
  git push origin main
  ```

  ---

  ## Conclusão

  O Git é uma ferramenta essencial para qualquer desenvolvedor.
  A prática constante é o melhor caminho para dominar o versionamento.

  > "Um bom histórico de commits conta a história do projeto."
  