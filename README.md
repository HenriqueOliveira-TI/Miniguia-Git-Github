Miniguia Git e GitHub
Sobre o projeto

Este projeto apresenta, de forma simples e prática, os principais conceitos de Git e GitHub para quem está começando na área de desenvolvimento de software.

O objetivo deste miniguia é ajudar estudantes e desenvolvedores iniciantes a compreender como funciona o controle de versões, como organizar alterações em um projeto e como utilizar o GitHub para compartilhar e colaborar no desenvolvimento.

O conteúdo foi construído durante o processo de estudo, utilizando o NotebookLM como ferramenta de apoio para organizar e compreender as informações presentes nas fontes selecionadas.

1. O que é Git?

O Git é um sistema de controle de versão distribuído.

De forma simples, ele permite registrar as alterações feitas nos arquivos de um projeto ao longo do tempo. Assim, é possível consultar versões anteriores, acompanhar o que foi alterado e recuperar uma versão anterior quando necessário.

Qual problema o Git resolve?

Antes de utilizar sistemas de controle de versão, era comum criar várias cópias de uma pasta para salvar diferentes versões de um projeto. Isso podia gerar confusão e até causar perda de informações.

Com o Git, as alterações ficam organizadas em um histórico, permitindo acompanhar a evolução do projeto de forma mais segura e organizada.

Exemplo

Imagine que você está desenvolvendo um site e alterou o título de uma página.

Você pode registrar essa alteração em um commit do Git. Se posteriormente perceber que a mudança causou algum problema, poderá consultar o histórico e recuperar uma versão anterior.

2. O que é GitHub?

O GitHub é uma plataforma utilizada para armazenar repositórios Git na internet.

Embora o Git seja uma ferramenta responsável pelo controle de versões no computador, o GitHub oferece um local remoto onde o projeto pode ser armazenado, compartilhado e utilizado em colaboração com outras pessoas.

Git e GitHub juntos

Um fluxo básico é:

Git no computador → Commit → Push → GitHub

Quando existem alterações no repositório remoto, podemos utilizar:

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

Repositório local x Repositório remoto
Repositório local	Repositório remoto
Fica no computador	Fica em um servidor
Usado durante o desenvolvimento	Usado para compartilhamento e colaboração
Pode ser utilizado sem internet na maior parte das operações	Normalmente depende da internet para sincronização
Guarda o histórico local	Recebe o histórico enviado pelo Git

4. Commit

Um commit é um registro de alterações no histórico do projeto.

Ele funciona como um ponto salvo na evolução do projeto. Cada commit pode possuir uma mensagem explicando o que foi alterado.

Quando criar um commit?

Um commit pode ser criado quando uma parte do trabalho estiver concluída, como:

Correção de um erro;
Criação de uma funcionalidade;
Alteração de uma página;
Atualização de documentação.
Staging Area

Antes do commit, as alterações podem ser colocadas na Staging Area, também chamada de área de preparação.

Ela permite selecionar quais alterações serão incluídas no próximo commit.

Fluxo

Alteração → Staging Area → Commit → Histórico

5. Branch

Uma Branch é uma linha de desenvolvimento separada dentro do projeto.

Ela permite trabalhar em uma funcionalidade, correção ou experimento sem alterar diretamente a versão principal.

Por que utilizar Branches?

As Branches auxiliam a:

Organizar o desenvolvimento;
Testar novas ideias;
Trabalhar em funcionalidades separadamente;
Permitir que várias pessoas trabalhem no mesmo projeto.

A Branch principal normalmente é chamada de main.

Exemplo

Imagine que o projeto possua uma versão estável na Branch main.

Para desenvolver uma nova funcionalidade, podemos criar uma Branch chamada:

nova-funcionalidade

O desenvolvimento acontece nessa nova Branch. Depois que a funcionalidade estiver pronta e testada, ela poderá ser integrada à Branch principal.

Fluxo

Main → Nova Branch → Desenvolvimento → Commits → Pull Request → Merge → Main

6. Merge

Merge significa unir alterações de diferentes Branches.

Ele é utilizado quando o trabalho realizado em uma Branch precisa ser incorporado a outra Branch.

Exemplo

Imagine que você criou uma Branch:

nova-funcionalidade

Depois de terminar o desenvolvimento, você pode realizar um Merge para incorporar essa funcionalidade à Branch principal.

Conflito de Merge

Um conflito acontece quando o Git encontra alterações diferentes em uma mesma parte do projeto e não consegue decidir sozinho qual deve permanecer.

Nesse caso, o desenvolvedor precisa analisar as alterações, escolher a solução adequada e finalizar o processo.

Fluxo

Main → Nova Branch → Desenvolvimento → Commits → Merge → Main atualizada

7. Pull Request

Um Pull Request, geralmente chamado de PR, é uma solicitação para que alterações realizadas em uma Branch sejam verificadas e incorporadas em outra Branch.

No GitHub, o Pull Request facilita a revisão das alterações antes da integração.

Exemplo

Você desenvolveu uma nova funcionalidade na Branch:

nova-funcionalidade

Depois de enviar essa Branch para o GitHub, você pode abrir um Pull Request solicitando que as alterações sejam incorporadas à Branch main.

Isso permite analisar as alterações antes de realizar o Merge.

8. Push

O comando git push envia os commits do repositório local para o repositório remoto.

Em um projeto hospedado no GitHub, o Push permite enviar para o GitHub os commits realizados no computador.

Exemplo

Você fez uma alteração no README:

Alteração → Staging Area → Commit → Push → GitHub

Depois do Push, os commits que estavam no repositório local passam a estar disponíveis no repositório remoto.

É possível fazer commit sem Push?

Sim.

O Git permite criar commits localmente sem enviá-los imediatamente para o GitHub.

9. Pull

O comando git pull é utilizado para trazer alterações do repositório remoto para o repositório local.

Ele é útil quando outras alterações foram enviadas para o repositório remoto e você precisa atualizar o seu computador.

Push x Pull

Push: computador → repositório remoto

Pull: repositório remoto → computador

Exemplo

Um colega envia uma alteração para o GitHub.

Você utiliza:

git pull

Assim, seu repositório local pode receber as alterações que estavam no repositório remoto.

10. Clone

O comando git clone é utilizado para criar uma cópia local de um repositório remoto.

Ele é muito utilizado quando você deseja começar a trabalhar em um projeto que já está hospedado no GitHub.

Exemplo

Um projeto está disponível no GitHub.

Você utiliza:

git clone

para copiar o repositório para o seu computador, incluindo as informações necessárias para trabalhar com o histórico do projeto.

Clone x Pull

Clone: utilizado para criar uma cópia local de um repositório remoto.

Pull: utilizado posteriormente para atualizar um repositório local que já existe.

11. Fluxo básico do Git e GitHub

Um fluxo simples pode ser representado assim:

Alteração → Staging Area → Commit → Push → Repositório remoto

Quando existem alterações no repositório remoto:

Repositório remoto → Pull → Computador

Em projetos que utilizam Branches:

Main → Nova Branch → Desenvolvimento → Commits → Pull Request → Merge → Main

12. Principais termos

Termo	Explicação simples
Git	Sistema de controle de versão
GitHub	Plataforma para hospedagem e colaboração com repositórios Git
Repositório	Local onde ficam os arquivos e o histórico do projeto
Commit	Registro de uma alteração no histórico
Staging Area	Área onde são preparadas as alterações para o próximo commit
Branch	Linha separada de desenvolvimento
Merge	União de alterações entre Branches
Pull Request	Solicitação para analisar e integrar alterações
Push	Envio de commits para o repositório remoto
Pull	Recebimento de alterações do repositório remoto
Clone	Criação de uma cópia local de um repositório remoto

13. Aprendizados

Durante a construção deste miniguia, foram estudados conceitos fundamentais de Git e GitHub e colocados em prática no próprio repositório.

O processo também ajudou a compreender que aprender Git não significa apenas memorizar comandos. É importante entender o fluxo de trabalho e saber quando cada recurso deve ser utilizado.

A utilização do GitHub também permitiu praticar conceitos como Branch, Commit, Push, Pull Request e Merge em uma situação real de desenvolvimento.

14. Cicatrizes de aprendizado

Durante o desenvolvimento do projeto, alguns erros e dificuldades fizeram parte do processo de aprendizagem.

Entre eles estiveram dúvidas sobre Branches, Commits, Pull Requests, Merge e a diferença entre Git e GitHub.

Essas dificuldades foram utilizadas como parte do aprendizado, permitindo compreender melhor o funcionamento das ferramentas na prática.

Os erros encontrados também mostraram a importância de realizar alterações de forma organizada, utilizar mensagens de commit claras e compreender o fluxo entre o repositório local e o repositório remoto.

## 15. Curadoria de Fontes

Para a construção deste miniguia, foram selecionadas fontes abertas e confiáveis relacionadas ao Git e ao GitHub. Essas fontes foram adicionadas ao NotebookLM e utilizadas como base para estudar, comparar e organizar as informações apresentadas neste projeto.

### Fontes utilizadas

1. **GitHub Docs — Documentação oficial do GitHub**
   https://docs.github.com/pt

2. **Pro Git — Livro sobre Git**
   https://git-scm.com/book/pt-br/v2

3. **Git Documentation — Documentação oficial do Git**
   https://git-scm.com/docs

As fontes foram escolhidas por apresentarem informações diretamente relacionadas aos conceitos estudados no miniguia, incluindo repositórios, commits, branches, merge, Pull Request e os comandos básicos do Git. A documentação oficial do Git apresenta, por exemplo, comandos relacionados a commits, branches, merge, pull e push. A documentação do GitHub também reúne conteúdos sobre repositórios e Pull Requests.

## 16. Engenharia de Prompts e uso do NotebookLM

Durante a construção do miniguia, o NotebookLM foi utilizado como ferramenta de apoio à aprendizagem e organização do conhecimento.

As perguntas foram elaboradas com o objetivo de compreender os conceitos de Git e GitHub de forma simples, identificar diferenças entre os recursos e organizar as informações para estudantes iniciantes.

### Prompts utilizados

**Prompt 1 — Conceitos fundamentais**

> Explique os principais conceitos de Git e GitHub para uma pessoa que está começando na área de desenvolvimento de software. Utilize uma linguagem simples e apresente exemplos práticos.

**Prompt 2 — Diferenças entre conceitos**

> Explique de forma simples a diferença entre Git e GitHub, repositório local e remoto, commit, branch, merge, Pull Request, push, pull e clone.

**Prompt 3 — Fluxo de trabalho**

> Apresente um fluxo básico de utilização do Git e GitHub, desde uma alteração realizada em um arquivo até o envio para o repositório remoto.

**Prompt 4 — Organização do miniguia**

> Organize os principais conceitos de Git e GitHub em uma estrutura de miniguia para estudantes iniciantes, incluindo explicações simples, exemplos práticos, glossário e fluxo de trabalho.

### Variação e refinamento dos prompts

Durante o processo, os prompts foram ajustados para obter respostas mais claras, organizadas e adequadas ao objetivo do projeto.

Em vez de utilizar apenas perguntas genéricas, foram solicitadas explicações com exemplos, comparações e organização por tópicos. Esse processo ajudou a transformar informações técnicas em um material mais fácil de compreender.

### Resultado do uso dos prompts

As respostas obtidas no NotebookLM serviram como apoio para compreender os conceitos, comparar informações presentes nas fontes selecionadas e organizar o conteúdo final do miniguia.

O conteúdo produzido pela IA não foi utilizado apenas de forma automática. As informações foram analisadas e organizadas de acordo com o objetivo do projeto e com as fontes utilizadas no NotebookLM.

## 17. Troubleshooting e Prompts Reutilizáveis

### Troubleshooting

Durante a elaboração do projeto, algumas dificuldades foram encontradas durante o uso do GitHub e do NotebookLM.

Uma das principais dificuldades foi compreender a diferença entre Git e GitHub e entender o papel de recursos como commit, branch, merge e Pull Request.

Também foi necessário ajustar os prompts utilizados no NotebookLM para obter respostas mais organizadas, claras e adequadas ao objetivo do miniguia.

Outro aprendizado importante foi compreender que a resposta fornecida pela Inteligência Artificial precisa ser analisada e comparada com as fontes utilizadas. A IA foi utilizada como ferramenta de apoio ao estudo, e não como substituta da análise das informações.

### Prompts reutilizáveis

Os prompts abaixo podem ser utilizados em futuras revisões ou estudos sobre Git e GitHub:

**Prompt 1 — Revisão**

> Revise os principais conceitos de Git e GitHub e explique de forma simples quais são as funções de cada recurso.

**Prompt 2 — Exercícios práticos**

> Crie exercícios práticos para treinar Git e GitHub, começando por comandos básicos e avançando gradualmente para branches, merge e Pull Requests.

**Prompt 3 — Identificação de erros**

> Analise este problema relacionado ao Git ou GitHub, explique a possível causa e apresente uma solução passo a passo utilizando uma linguagem simples.

**Prompt 4 — Revisão para iniciantes**

> Faça uma revisão dos principais conceitos de Git e GitHub para iniciantes, apresentando exemplos práticos e destacando os pontos que costumam gerar dúvidas.

### Conclusão

A construção deste miniguia permitiu utilizar o NotebookLM como uma ferramenta de aprendizagem ativa, combinando curadoria de fontes, elaboração de prompts, análise das respostas e organização do conhecimento.

O projeto também possibilitou praticar Git e GitHub durante sua própria construção, tornando o aprendizado mais próximo de uma situação real de desenvolvimento.
