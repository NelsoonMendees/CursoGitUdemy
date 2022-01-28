# Curso Git / GitHub

### Udemy

- Por ser um sistema de gerenciamento de controle de versão de código / documentos, o git possui recursos avançados de monitoramento e acompanhamento de arquivos que fazem parte de um projeto. Ou seja, após ativo em um projeto, o git começa a monitorar as mudanças ocorridas neste projeto e nos mostra através de um poderoso sistema de estágios(ou fases) em que o estágio ou fase que se encontram os arquivos.

- **Ciclo de vida dos status de arquivos no Git**
  
  - **Untracked**: Significa que apesar do arquivo fazer parte do projeto, ele ainda não foi adicionado ao monitoramento do git.
    
    - OBS: Enquanto não houver monitoramento do arquivo, o git não estará controlando o versionamento deste arquivo. É como se o arquivo apresar de estar no projeto não faz parte do mesmo.

- **Tracked**: O git passa a controlar as mudanças neste arquivo. Arquivos com este estado são conhecidos como "new file".

- **Modified**: Quando modificamos um arquivo que está rastreado, seu status passa a ser "modificado". Desta forma sabemos facilmente se um arquivo não esta rastreado, ou se está rastreado mas ocorreu modificações.
  
  - OBS: é nesta etapa que podem ocorrer conflitos, pois imaginando que você e outra pessoa baixaram uma cópia do mesmo arquivo e ambos o modificaram, de alguma forma o arquivo deve ser juntado ao final para gerar apenas um atualizado.

- **Staged**: Quando um arquivo está pronto, ou seja, ele já está sendo rastreado e já foi modificado e finalizado, então está pronto para ser enviado para o repositório, então o status passa a ser "Staged" ou "Preparado". Os arquivos são enviados para o repositório através de commits.

# **Comandos Git - Git Básico**

- Configuração de usuário - Local
  
  - git config user.name "Nome"
  
  - git config user.e-mail "e-mail"
    
    - Para adicionar usuário e e-mail de forma global, adicionar **--global** antes do user.
  
  - git status: mostra o status dos arquivos do repositório
  
  - git add nomeDoArquivo: adiciona o arquivo par ao git monitorar
  
  - git commit -m "comentário": faz o commit dos arquivos para o repositório.
  
  - git log: exibe todo o histórico de commits realizados.
  
  - git checkout 12e8b56(numero da branch): "volta no tempo" no projeto.
    
    - Cuidado para não perder arquivos. Não modificar nada! Para voltar ao principal:
      
      - git checkout master
  
  - git mv nomeArquivo novoNome: altera o nome do arquivo especificado.
  
  - git diff --staged: mostra as alterações no arquivo que **Ainda não foram commitadas!**
  
  - git diff 43426cc(numero da branch): mostra as diferenças entre o arquivo atual e uma branch especifica
  
  - git commit --amend -m "descrição": faz a correção do ultimo commit realizado caso tenha algum erro na descrição do commit ou queira enviar outro arquivo junto.
  
  - git restore --staged nomeDoArquivo: remove o status de staged.
  
  - git checkout nomeDoArquivo: remove as alterações realizadas no arquivo para o ultimo commit.
  
  - git reset HEAD --hard: reseta todas as alterações realizadas no projeto para o ultimo commit.

# Git Intermediário

- Branch nada mais é do que a ramificação do projeto
  
  - Branch master - ramo principal
  
  - git branch: mostra todas as branchs do repositório
  
  - git checkout nomeDaBranch: altera a branch que deseja trabalhar.
  
  - git merge nomeDaBranch: realiza a junção das branchs do repositorio.
  
  - git clone: faz uma copia(clone) de um repositorio.





# Git Avançado


