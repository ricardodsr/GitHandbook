<h1>Git é um sistema distribuido de gestão para código fonte e controlo de versões.</h1>
<h3>Funciona através de uma série de registos de estado do projecto e usa esse registo para permitir funcionalidades de versionamento e gestão de código fonte.</h3>

<h3>Conceitos de versionamento</h3>
O que é controlo de versões: <br>
Controlo de versões (source control) é um processo de registo de alterações a um ficheiro ou conjunto de ficheiros ao longo do tempo.<br>

Controlo de versões: Centralizado VS Distribuido.<br>
Controlo de versões centralizado foca-se na sincronização, registo e backup de ficheiros.<br>
Controlo de versões distribuido foca-se em partilhar alterações. Cada alteração é associada a um id único.<br>
Sistemas distribuidos não têm estrutura definida. É possivel ter um sistema centralizado ao estilo SVN usando git.<br>


<h3>Porquê usar git?</h3></br>
Permite trabalhar offline.</br>
Colaborar com outros é fácil!</br>
Criar branches é fácil!</br>
Fazer merge é fácil!</br>
Git é rápido.</br>
Git é flexivel.</br>
Git - Arquitectura</br>

<h3>Repositório é :</h3>
Um conjunto de ficheiros, directórios, registos históricos, commits e referências. Pode ser imaginado como uma estrutura de dados de código fonte com a particularidade de cada elemento do código fonte permitir acesso ao histórico das suas alterações, entre outras coisas.
Um repositório git é constituido pelo directório .git e a working tree


<h3>Directório .git (componente do repositório)</h3>
O repositório .git contém todas as configurações, logs, branches, referências e outros.

<h3>Working Tree (componente do repositório)</h3>
Isto é basicamente os directórios e ficheiros do repositório. É frequentemente referido como o directório do projecto.

<h3>Index (componente do directório .git)</h3>
O Index é a camada de interface no git. Consistente num elemento que separa o directório do projecto do repositório git. Isto permite aos programadores um maior controlo sobre o que é registado no repositório git.

<h3>Commit</h3>
Um commit* de git é um registo de um cojunto de alterações ou manipulações nos ficheiros do projecto. Por exemplo, ao adicionar cinco ficheiros e remover outros 2, estas alterações serão gravadas num commit (ou registo). Este commit pode então ser enviado para outros repositórios ou não!

<h3>Branch</h3>
Um branch é essencialmente uma referência que aponta para o último commit efetuado. À medida que são feitos novos commits, esta referência é atualizada automaticamente e passa a apontar para o commit mais recente.

<h3> HEAD e head (componentes do directório .git) </h3>
HEAD é a referência que aponta para o branch em uso. Um repositório só tem uma HEAD activa. head é uma referência que aponta para qualquer commit. Um repositório pode ter um número indefinido de heads
