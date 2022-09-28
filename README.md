# Git

Git é um sistema distribuido de gestão para código fonte e controlo de versões.

Funciona através de uma série de registos de estado do projecto e usa esse registo para permitir funcionalidades de versionamento e gestão de código fonte.

Conceitos de versionamento
O que é controlo de versões
Controlo de versões (source control) é um processo de registo de alterações a um ficheiro ou conjunto de ficheiros ao longo do tempo.

Controlo de versões: Centralizado VS Distribuido
Controlo de versões centralizado foca-se na sincronização, registo e backup de ficheiros.
Controlo de versões distribuido foca-se em partilhar alterações. Cada alteração é associada a um id único.
Sistemas distribuidos não têm estrutura definida. É possivel ter um sistema centralizado ao estilo SVN usando git.


Porquê usar git?
Permite trabalhar offline.
Colaborar com outros é fácil!
Criar branches é fácil!
Fazer merge é fácil!
Git é rápido.
Git é flexivel.
Git - Arquitectura
Repositório

Um conjunto de ficheiros, directórios, registos históricos, commits e referências. Pode ser imaginado como uma estrutura de dados de código fonte com a particularidade de cada elemento do código fonte permitir acesso ao histórico das suas alterações, entre outras coisas.

Um repositório git é constituido pelo directório .git e a working tree

Directório .git (componente do repositório)
O repositório .git contém todas as configurações, logs, branches, referências e outros.

Working Tree (componente do repositório)
Isto é basicamente os directórios e ficheiros do repositório. É frequentemente referido como o directório do projecto.

Index (componente do directório .git)
O Index é a camada de interface no git. Consistente num elemento que separa o directório do projecto do repositório git. Isto permite aos programadores um maior controlo sobre o que é registado no repositório git.

Commit
Um commit* de git é um registo de um cojunto de alterações ou manipulações nos ficheiros do projecto. Por exemplo, ao adicionar cinco ficheiros e remover outros 2, estas alterações serão gravadas num commit (ou registo). Este commit pode então ser enviado para outros repositórios ou não!

Branch
Um branch é essencialmente uma referência que aponta para o último commit efetuado. À medida que são feitos novos commits, esta referência é atualizada automaticamente e passa a apontar para o commit mais recente.

HEAD e head (componentes do directório .git)
HEAD é a referência que aponta para o branch em uso. Um repositório só tem uma HEAD activa. head é uma referência que aponta para qualquer commit. Um repositório pode ter um número indefinido de heads
