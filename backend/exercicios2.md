**1.** O que é o **Node.js**?
Explique sua finalidade e por que ele é considerado um ambiente de execução e não uma linguagem de programação.

--O Node.js é um ambiente de execução (runtime environment) de código aberto e multiplataforma que permite executar código JavaScript fora de um navegador web, geralmente no servidor-

**2.** Qual a diferença entre **Node.js** e **JavaScript executado no navegador**?
Cite pelo menos **duas diferenças**.

A principal diferença entre Node.js e JavaScript no navegador é o ambiente de execução (runtime). Enquanto o navegador é projetado para rodar scripts no lado do cliente (front-end) para interagir com o usuário, o Node.js é um ambiente que permite executar JavaScript diretamente no servidor (back-end), acessando recursos do sistema operacional. 


**3.** O que é o **V8 Engine** e qual sua importância para o funcionamento do Node.js?
O V8 Engine é um mecanismo (engine) de JavaScript e WebAssembly de alto desempenho, código aberto, desenvolvido pelo Google em C++. Ele é o motor que interpreta e compila o código JavaScript diretamente em código de máquina nativo (native machine code), o que o torna incrivelmente rápido. Embora tenha sido criado para o navegador Google Chrome, o V8 é independente do navegador e pode ser incorporado em qualquer aplicação C++, como o Node.js. 

**4.** Explique o conceito de **I/O não bloqueante** no Node.js.
Por que isso melhora o desempenho de aplicações?

O I/O não bloqueante (ou E/S não bloqueante - Entrada/Saída) é um dos pilares fundamentais do Node.js. Ele permite que o ambiente de execução inicie uma operação de I/O (leitura de arquivos, requisições de rede, consultas a banco de dados) e continue processando outras tarefas sem esperar que essa operação seja concluída. 

**5.** O que é o **Event Loop**?
Descreva, de forma resumida, como ele funciona.

O Event Loop (Loop de Eventos) é um mecanismo fundamental no ambiente de execução do JavaScript (como navegadores e Node.js) que permite que a linguagem realize operações assíncronas e não bloqueantes, mesmo sendo single-threaded (executa uma coisa de cada vez). 

**6.** O que são **módulos** no Node.js?
Explique a diferença entre:

* Módulos internos
* Módulos externos
* Módulos criados pelo desenvolvedor

Módulos no Node.js são arquivos ou bibliotecas JavaScript independentes que organizam, encapsulam e reutilizam código, permitindo dividir aplicações complexas em partes menores. Eles facilitam a manutenção, importando funcionalidades específicas de um arquivo para outro, geralmente via require (CommonJS) ou import (ES Modules). 

**7.** Para que serve o arquivo **package.json** em um projeto Node.js?
Cite pelo menos **três informações** que ele pode conter.

O arquivo package.json é um componente fundamental em projetos Node.js, agindo como um "manifesto" ou centralizador de configurações. Ele serve para armazenar metadados do projeto, gerenciar as dependências (bibliotecas externas) que o projeto utiliza e definir scripts para automação de tarefas. 

**8.** O que é o **npm**?
Explique sua função no desenvolvimento de aplicações Node.js.

O npm (Node Package Manager) é o gerenciador de pacotes padrão para o ambiente de execução Node.js e é, atualmente, um dos maiores repositórios de software de código aberto do mundo. Ele vem incluído automaticamente quando você instala o Node.js. 

**9.** O que é uma **API REST** e como o Node.js pode ser usado para desenvolvê-la?

Uma API REST (Representational State Transfer) é um estilo arquitetural para sistemas distribuídos, como a web, que define um conjunto de diretrizes para a criação de serviços web. Ela permite que diferentes aplicações (clientes e servidores) troquem dados de forma leve, padronizada e segura, utilizando o protocolo HTTP. 

**10.** Cite **duas vantagens** e **duas desvantagens** do uso do Node.js em aplicações web.

O Node.js é amplamente utilizado no desenvolvimento web, especialmente devido ao uso de JavaScript no backend. Abaixo estão duas vantagens e duas desvantagens principais: 
