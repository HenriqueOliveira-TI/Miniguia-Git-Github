Miniguia Git e GitHub
Sobre o projeto

Este projeto apresenta, de forma simples e prática, os principais conceitos de Git e GitHub para quem está começando na área de desenvolvimento de software.

O objetivo deste miniguia é ajudar estudantes e desenvolvedores iniciantes a compreender como funciona o controle de versões, como organizar alterações em um projeto e como utilizar o GitHub para compartilhar e colaborar no desenvolvimento.

O conteúdo foi construído durante o processo de estudo, utilizando o NotebookLM como ferramenta de apoio para organizar e compreender as informações presentes nas fontes selecionadas.

1. O que é Git?

O Git é um sistema de controle de versão distribuído.

De forma simples, ele permite registrar as alterações feitas nos arquivos de um projeto ao longo do tempo. Assim, é possível consultar versões anteriores, acompanhar o que foi alterado e recuperar uma versão anterior quando necessário.

Qual problema o Git resolve?

Antes de utilizar sistemas de controle de versão, era comum criar várias cópias de uma pasta para guardar diferentes versões de um projeto. Isso podia gerar confusão e até causar perda de informações.

Com o Git, as alterações ficam organizadas em um histórico.

Exemplo

Imagine que você está desenvolvendo um site e altera o título de uma página.

Você pode registrar essa alteração no Git. Se posteriormente perceber que a mudança causou um problema, poderá consultar o histórico e recuperar uma versão anterior.

2. O que é GitHub?

O GitHub é uma plataforma utilizada para hospedar repositórios Git na internet.

Enquanto o Git é a ferramenta responsável pelo controle de versões no computador, o GitHub oferece um local remoto onde o projeto pode ser armazenado, compartilhado e utilizado em colaboração com outras pessoas.

Git e GitHub trabalham juntos

Um fluxo comum é:

Git no computador → Commit → Push → GitHub

Quando outra pessoa envia alterações para o GitHub, podemos utilizar:

GitHub → Pull → Computador

3. Repositório

Um repositório é o local onde o Git armazena os arquivos e o histórico de alterações de um projeto.

O repositório contém as informações necessárias para acompanhar a evolução do projeto.

Repositório local

É o repositório que fica no computador do desenvolvedor.

Nele é possível realizar alterações, criar commits e consultar o histórico sem depender de uma conexão constante com a internet.

Repositório remoto

É o repositório armazenado em um servidor ou plataforma online, como o GitHub.

Ele facilita o compartilhamento, a colaboração e a manutenção de uma cópia do projeto fora do computador local.

Comparação
Repositório local	Repositório remoto
Fica no computador	Fica em um servidor
Usado durante o desenvolvimento	Usado para compartilhamento e colaboração
Pode funcionar sem internet	Normalmente depende da conexão para sincronização
Guarda o histórico local	Pode receber o histórico enviado pelo Git
4. Commit

Um commit é um registro de alterações no histórico do projeto.

Ele funciona como um ponto salvo na evolução do projeto. Cada commit pode possuir uma mensagem explicando o que foi alterado.

Quando criar um commit?

Um commit pode ser criado quando uma parte do trabalho estiver concluída, como:

correção de um erro;
criação de uma funcionalidade;
alteração de uma página;
atualização de documentação.
Staging Area

Antes do commit, as alterações podem ser colocadas na Staging Area, também chamada de área de preparação.

Ela permite selecionar quais alterações serão incluídas no próximo commit.

Fluxo

Alteração → Staging Area → Commit → Histórico

5. Branch

Uma branch é uma linha de desenvolvimento separada dentro do projeto.

Ela permite trabalhar em uma funcionalidade, correção ou experimento sem alterar diretamente a versão principal.

Por que utilizar branches?

Branches ajudam a:

organizar o desenvolvimento;
testar novas ideias;
trabalhar em funcionalidades separadamente;
permitir que várias pessoas trabalhem no mesmo projeto.

A branch principal normalmente é chamada de main.

Exemplo

Imagine que o projeto possui uma versão estável na branch main.

Para desenvolver uma nova funcionalidade, podemos criar:

nova-funcionalidade

O desenvolvimento acontece nessa nova branch. Depois que a funcionalidade estiver pronta e testada, ela poderá ser integrada à main.

Fluxo

Branch main → Nova branch → Desenvolvimento → Commits → Conclusão

6. Merge

Merge significa unir alterações de diferentes branches.

Ele é utilizado quando o trabalho realizado em uma branch precisa ser incorporado a outra branch.

Exemplo

Imagine que você criou a branch:

nova-funcionalidade

Depois de terminar o desenvolvimento, você pode realizar um merge para incorporar essa funcionalidade à main.

Conflito de merge

Um conflito acontece quando o Git encontra alterações diferentes em uma mesma parte do projeto e não consegue decidir sozinho qual deve permanecer.

Nesse caso, o desenvolvedor precisa analisar as alterações, escolher a solução adequada e finalizar o processo.

Fluxo

Branch main → Nova branch → Desenvolvimento → Commits → Merge → Main atualizada

7. Pull Request

Um Pull Request, geralmente chamado de PR, é uma solicitação para que as alterações realizadas em uma branch sejam analisadas e incorporadas a outra branch.

No GitHub, o Pull Request facilita a revisão do código antes da integração.

Exemplo

Você desenvolveu uma nova funcionalidade na branch:

nova-funcionalidade

Depois de enviar essa branch para o GitHub, pode abrir um Pull Request solicitando que as alterações sejam incorporadas à main.

Isso permite que o trabalho seja analisado antes do merge.

8. Push

O comando git push envia os commits do repositório local para o repositório remoto.

Em um projeto hospedado no GitHub, o push permite enviar para o GitHub os commits realizados no computador.

Exemplo

Você fez uma alteração no README:

Alteração → Staging Area → Commit → Push → GitHub

Depois do push, os commits que estavam no repositório local passam a estar disponíveis no repositório remoto.

É possível fazer commit sem push?

Sim.

O Git permite criar commits localmente sem enviá-los imediatamente para o GitHub.

9. Pull

O comando git pull é utilizado para trazer alterações do repositório remoto para o repositório local.

Ele é útil quando outras alterações foram enviadas para o repositório remoto e você precisa atualizar seu computador.

Push x Pull

Push: computador → repositório remoto

Pull: repositório remoto → computador

Exemplo

Um colega envia uma alteração para o GitHub.

Você utiliza:

git pull

Assim, o seu repositório local pode receber as alterações que estavam no repositório remoto.

10. Clone

O comando git clone é utilizado para criar uma cópia local de um repositório remoto.

Ele é muito utilizado quando você deseja começar a trabalhar em um projeto que já está hospedado no GitHub.

Exemplo

Um projeto está disponível no GitHub.

Você utiliza git clone para copiar o repositório para o seu computador, incluindo as informações necessárias para trabalhar com o histórico do projeto.

Clone x Pull

Clone: utilizado para criar uma cópia local de um repositório remoto.

Pull: utilizado posteriormente para atualizar um repositório local que já existe.

11. Fluxo básico do Git e GitHub

Um fluxo simples pode ser representado assim:

Alteração → Staging Area → Commit → Push → Repositório remoto

Quando existem alterações no repositório remoto:

Repositório remoto → Pull → Computador

Em projetos que utilizam branches:

Main → Nova branch → Desenvolvimento → Commits → Pull Request → Merge → Main

12. Principais termos
Termo	Explicação simples
Git	Sistema de controle de versão
GitHub	Plataforma para hospedagem e colaboração com repositórios Git
Repositório	Local onde ficam os arquivos e o histórico do projeto
Commit	Registro de uma alteração no histórico
Staging Area	Área onde são preparadas as alterações para o próximo commit
Branch	Linha separada de desenvolvimento
Merge	União de alterações entre branches
Pull Request	Solicitação para analisar e integrar alterações
Push	Envio de commits para o repositório remoto
Pull	Recebimento de alterações do repositório remoto
Clone	Criação de uma cópia local de um repositório remoto
13. Aprendizados

Durante a construção deste miniguia, foram estudados conceitos fundamentais de Git e GitHub e colocados em prática no próprio repositório.

O processo também ajudou a compreender que aprender Git não significa apenas memorizar comandos. É importante entender o fluxo de trabalho e saber quando cada recurso deve ser utilizado.

14. Cicatrizes de aprendizado

Durante o desenvolvimento do projeto, alguns erros e dificuldades fizeram parte do processo de aprendizagem.

Entre eles estiveram dúvidas sobre branches, commits, Pull Requests e a diferença entre Git e GitHub.

Essas dificuldades foram utilizadas como parte do aprendizado, permitindo compreender melhor o funcionamento das ferramentas na prática.

15. Fontes

As informações utilizadas neste miniguia foram estudadas e organizadas com o auxílio do NotebookLM, utilizando as fontes selecionadas no notebook.

As principais referências utilizadas foram materiais relacionados à documentação oficial do Git e do GitHub.

O objetivo foi utilizar as fontes como base para compreender os conceitos e transformar o conteúdo técnico em uma explicação mais simples para estudantes iniciantes.
