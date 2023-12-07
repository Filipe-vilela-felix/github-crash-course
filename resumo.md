# Resumo do Tutorial

## Iniciando com git init

### Iniciando no próprio VS Code:

- No terminal do VS Code, digito `git init` para inicializar o repositório Git.

### Iniciando dentro da linha de comando do Git:

- Dentro dessa linha de comando, digitar `git init` e dar enter.
  Porém, nada acontece visualmente dentro da minha pasta, isso porque os arquivos do Git estão escondidos. Para torná-los visíveis...
- No "Painel de Controle" dos arquivos, clicar em "View" ou "Visualizar" e marcar "Itens Ocultos".
  Obs: O arquivo `.git` que tornará a aparecer não deve ser modificado!

## Criando um Novo Commit no Git

- Após realizar algumas alterações significativas no seu código, como terminar um trabalho em um recurso específico, corrigir um bug ou algo semelhante, é hora de criar um novo commit. O processo envolve duas etapas principais: `git add` e `git commit`.

### 1ª Etapa: git add <file(s)>

- Você adiciona os arquivos que contêm as alterações que devem ser incluídas nesse commit. Isso permite que você controle quais arquivos e      alterações farão parte de um determinado commit. Este processo é conhecido como staging, onde você prepara as mudanças que serão incluídas no próximo commit.

- Existem várias maneiras de adicionar todos os arquivos presentes, se necessário. Por exemplo: Ex: git add another.txt another2.txt

- Se os arquivos estiverem em uma subpasta, você pode especificar o nome dessa subpasta, e todos os arquivos dentro dela serão adicionados: 
    Ex: git add  subfolder/

**Observação:** Você pode verificar o status atual do seu repositório Git com o comando `git status`. A primeira coisa que aparecerá é "On branch master/main", indicando que você está no ramo principal.

### 2ª Etapa: git commit -m "mensagem"

- Isso cria um commit com base nas alterações que foram preparadas (staged). Entre as aspas, você digita uma mensagem curta que descreve o commit. Por exemplo: git commit -m “Adiciona nova funcionalidade”

**Observação:** O primeiro commit criado, seguindo um padrão organizacional, é geralmente chamado de "initial commit".

Esses dois comandos juntos formam um commit. No entanto, eles são separados para que você não tenha que incluir todas as alterações em todos os arquivos sempre que criar um novo commit.

**Observação:** Sempre que você iniciar um novo projeto ou repositório Git, é recomendável criar um commit inicial, comumente referido como "initial commit".    

## Navegando pelo Histórico de Commits no Git

### git log

- Para obter uma lista de todos os commits criados até então, bem como seus respectivos IDs, você pode usar o comando `git log`. Após a execução do `git log`, é possível notar que ele informa qual branch você está usando.

**Observação:** O ponteiro `HEAD` indica qual estado está carregado no momento. Você também pode começar a se mover entre os commits usando o comando `git checkout <ID>`.