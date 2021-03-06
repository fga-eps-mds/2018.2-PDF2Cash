# Documento de visão
***

## Histórico de Revisão
***

| Data | Versão | Descrição | Autor |
|:----:|:------:|:---------:|:-----:|
| 25/08/18 | 0.1 | Abertura do Documento de Visão | Brian Lui |
| 26/08/18 | 0.2 | Introdução | Brian Lui |
| 28/08/18 | 0.3 | Posicionamento | Wictor Girardi |
| 29/08/18 | 0.4 | Visão Geral Do Produto | Rafael Teodosio |
| 31/08/18 | 0.5 | Descrição dos Envolvidos e dos Usuários | Lucas Gomes |
| 03/09/18 | 0.5.1 | Mudança dentro do posicionamento | Wictor Girardi |
| 03/09/18 | 0.5.2 | Adição de Descrição dos Envolvidos e dos Usuários | Lucas Gomes |
| 05/09/18 | 0.5.3 | Adição de recursos do produto | Wictor Girardi |
| 05/09/18 | 0.6 | Restrições | Julio Litwin |
| 05/09/18 | 0.7 | Intervalos de Qualidade | Luis Claudio T. Lima |
| 07/09/18 | 0.8 | Revisão geral do documento | Brian Lui, Julio Litwin, Lucas Gomes, Luis Claudio, Wictor Girardi, Rafael Teodosio   |
| 07/09/18 | 1.0 | Documento estável | Brian Lui, Julio Litwin, Lucas Gomes, Luis Claudio, Wictor Girardi, Rafael Teodosio |
| 20/09/18 | 1.1 | Correção da Finalidade e Escopo | Brian Lui |
| 20/09/18 | 1.2 | Correção da Visão Geral do Produto | Rafael Teodosio |
| 21/09/18 | 1.3 | Correção do Posicionamento | Wictor Girardi |
| 21/09/18 | 1.4 | Correção das Descrições dos Envolvidos e dos Usuários | Lucas Gomes |
|22/11/18 | 1.5 | Revisão de Documento | Luís Cláudio T. Lima
***
## 1. Introdução
***

Esta documentação tem como propósito coletar, analisar e definir os insumos necessários para a realização do PDF2CASH, que é uma ferramenta para gerar dados a partir de notas fiscais eletrônicas(NFe). Sendo possível o armazenamento e a organização.
Nesta introdução será apresentada uma visão geral para o entendimento do projeto, de tal modo que fique claro para todos os recursos necessários e as razões que levam a essas necessidades.

### 1.1 Finalidade

Este documento tem como objetivo definir os requisitos, necessidades e os recursos necessários, especificamente os de alto nível, para que o investidor possa compreender e tenha o completo entendimento do projeto PDF2CASH.

### 1.2 Escopo

Neste documento serão abordados os pontos necessários para o desenvolvimento do PDF2CASH, de tal modo que o produto será de fácil entendimento para pessoas leigas. Resumidamente, este software será utilizado no setor financeira de micro empresas gerando dados a partir de notas fiscais eletrônicas, primeiramente sendo realizada a leitura automatizada do pdf, o armazenamento dos dados, o gerenciamento dos gastos e a geração de gráficos de análise financeira respectivamente. Em relação ao controle de segurança, foi determinado que os funcionários da parte financeira terão acesso apenas as notas fiscais da empresa em que trabalha.

### 1.3 Definições, Acrônimos e Abreviações

Alguns termos e conceitos serão necessários para a concepcao do total entendimento deste documento e estao listados logo abaixo :

  1. PDF(Portable Document Format): É um formato de arquivo usado para exibir e compartilhar documentos de maneira compatível.
  2. NFe (Nota Fiscal Eletrônica): Arquivo eletrônico com o objetivo de substituir a tradicional nota fiscal em papel, onde contém as informações fiscais da operação comercial.
  3. HD(Hard Disk): Sistema de armazenamento de alta capacidade destinado ao armazenamento de arquivos e programas.
  4. PO (Product Owner): Membro responsável por compreender a idéia e ser os “olhos” do cliente dentro do projeto.
  5. CTe (Conhecimento de Transporte Eletrônico): Documento digital, para fins fiscais, onde é documentado prestação de serviço de transporte de cargas realizadas por qualquer modal.
  6. CNPJ (Cadastro Nacional da Pessoa Jurídica): Número único que identifica uma pessoa jurídica.
  7. Backup: Cópia de um ou mais arquivos onde será guardado em dispositivo de armazenamento ou diretório diferente do arquivo original.
  8. Parser: É um componente de compilador ou interpretador que atua no processo de análise de sentenças e sequências de palavras ou símbolos mostrando sua relação sintática ou semântica entre si para conversão em informações.  

### 1.4 Referências

WARNOCK, John. Adobe. Disponível em: <https://acrobat.adobe.com/br/pt/acrobat/about-adobe-pdf.html>. Acesso em: 29 ago. 2018.
Desconhecido. Sobre a NF-e. Disponível em: <http://www.nfe.fazenda.gov.br> Acesso em: 31 ago. 2018
Desconhecido. Conheça o CT-e. Disponível em: <http://www.cte.fazenda.gov.br/portal/principal.aspx> Acesso em: 31 ago. 2018

### 1.5 Visão Geral

Neste documento é definido o problema a ser resolvido de acordo com os requisitos do software previamente elaborados, o entendimento sobre os usuários e envolvidos, uma visão geral do produto a ser desenvolvido e dos recursos necessários.

***
## 2. Posicionamento
***

### 2.1 Oportunidade de Negócios

Atualmente diversas empresas enfrentam problemas relacionados ao seus controles de gastos e como consequência disso ocorre a dificuldade de maximização de lucros, levando em consideração o grande volume de vendas e compras realizadas, e algumas vezes por falta de experiência na coordenação econômica da empresa. Com base nesses problemas o PDF2CASH busca realizar, de maneira rápida e prática, a organização, armazenamento e geração de gráficos de dados baseados nas notas fiscais recebidas por essas empresas, gerando assim um maior controle de onde está sendo gasto o dinheiro e se está ocorrendo aumentos ou quedas no histórico monetário dessa empresa, além da prevenção de possíveis multas causadas pela falta de armazenamento das notas fiscais.

### 2.2 Descrição do Problema

<table>
  <tr><th>O problema de</th><td>Falta de praticidade no trabalho relacionado às notas fiscais que abrange a falta de organização e a falta de controle de gastos. </td></tr>
  <tr><th>Afeta</th><td>
A empresa de modo geral e principalmente seu setor financeiro.
</td></tr>
  <tr><th>Cujo impacto é</th><td>O setor financeiro da empresa já que não consegue de maneira prática manter a organização e controle de seus gastos e o armazenamento de suas notas fiscais, causando dano ao lucro geral da empresa.</td></tr>
  <tr><th>Uma boa solução seria</th><td>Uma aplicação prática e inteligente que reconhece notas fiscais emitidas e trabalha em cima delas gerando, de maneira automatizada, gráficos de gastos recentes ou mesmo dentro de um histórico e gerando um melhor entendimento de onde e porque está sendo gasto o dinheiro da empresa, juntamente com o armazenamento automático dessas notas, evitando assim burocracia e trabalho desnecessário, no intuito de realizar uma maximização de lucros da empresa.</td></tr>
</table>

### 2.3 Sentença de Posição do Produto

<table>
  <tr><th>Para</th><td>Microempresas, com ênfase no setor financeiro </td></tr>
  <tr><th>Que</th><td>
Possuem a necessidade de um software que realize de maneira automatizada, prática e organizada o controle de gastos por meio de gráficos e organização de notas fiscais sem a necessidade de interação humana durante o processo.
</td></tr>
  <tr><th>Nome do produto</th><td>PDF2CASH</td></tr>
  <tr><th>Diferente de</th><td>Noov e Arquivei</td></tr>
  <tr><th>Nosso produto</th><td>Gera dados úteis baseando-se na leitura nativa de arquivos PDF’s de notas fiscais eletrônicas de maneira automática e rápida por meio do nosso software livre, agrupando os gastos relacionados, gerando gráficos de história e realizando um armazenando seguro das notas fiscais nos bancos de dados da empresa. </td></tr>
</table>

***
## 3. Descrições dos Envolvidos e dos Usuários
***

### 3.1 Resumo dos Envolvidos
| Nome | Descrição | Responsabilidades |
|:----:|:---------:|:-----------------:|
| Investidores | Micro empresas com interesse em automatizar o controle de notas fiscais. | Avaliar a qualidade do produto no intuito de comprar o mesmo. |
| Equipe de desenvolvimento do projeto | Equipe de alunos de Métodos de Desenvolvimento de Software da UnB. | Planejar, desenvolver, testar, documentar e implementar o sistema. |
| Equipe de engenharia de produto | Equipe de alunos de Engenharia de Produto de Software da UnB. | Planejar, projetar e gerir o projeto. Onde a equipe é composta pelo PO, Scrum Master, DevOps e Arquiteto que desempenham os papéis de, respectivamente, compreender, guiar a equipe, estudar a implementação e, configurar o ambiente de desenvolvimento do projeto. |

### 3.2 Resumo dos Usuários
| Nome | Descrição | Responsabilidades | Envolvido |
|:----:|:---------:|:-----------------:|:---------:|
| Administrador | Operador do sistema com mais recurso para uso | Responsável por realizar cadastro de novos usuários e empresas e excluir nota fiscal. | Usuário |
| Funcionário Cadastrado | Operador do sistema | Responsável pela inserção dos PDFs das notas fiscais, visualização de análises e nota fiscal e listagem das notas fiscais. | Usuário |

### 3.3 Perfis dos Envolvidos

#### 3.3.1	Investidores
<table>
  <tr><th>Descrição</th><td>Investidor com o interesse em automatizar o gerenciamento de notas fiscais da empresa.</td></tr>
  <tr><th>Tipo</th><td>Conhecimento na área administrativa e financeira.</td></tr>
  <tr><th>Responsabilidades</th><td> Analisar, dar opinião e averiguar a utilização do produto em sua empresa.</td></tr>
  <tr><th>Critérios de Sucesso </th><td>Receber uma aplicação que possa suprir suas necessidades diante as notas fiscais de forma automatizada.</td></tr>
  <tr><th> Envolvimento </th><td> Alto </td></tr>
  <tr><th> Comentários / Problemas </th><td> - </td></tr>
</table>

#### 3.3.2	Equipe de Desenvolvedores
<table>
  <tr><th> Representantes </th><td>
  Brian Lui<br>
  Julio Cesar Litwin<br>
  Lucas Gomes Silva<br>
  Luis Claudio Telles Lima<br>
  Rafael Santos Teodosio<br>
  Wictor Bastos Girardi<br></td></tr>
  <tr><th>Descrição</th><td>Desenvolvedores do projeto</td></tr>
  <tr><th>Tipo</th><td> Graduandos de Engenharia de Software na Universidade de Brasília, matriculados na disciplina de Métodos de Desenvolvimento de Software.</td></tr>
  <tr><th>Responsabilidades</th><td>Planejar o sistema, realizar testes de implementação, documentar a estrutura do software e implementar o sistema de acordo com a documentação.</td></tr>
  <tr><th>Critérios de Sucesso</th><td>Desenvolver o sistema dentro do prazo estimado e adquirir novos conhecimentos sobre desenvolvimento de software.</td></tr>
  <tr><th>Envolvimento</th><td>Alto</td></tr>
  <tr><th>Comentários / Problemas</th><td>-</td></tr>
</table>

#### 3.3.3	Equipe de Desenvolvedores
<table>
  <tr><th>Representantes</th><td>Bruno Matias Casas<br>
  Carlos Enrique Rodrigues Aragon<br>
  Daniel Marques Rangel<br>
  Francisco Wallacy Coutinho Braz<br></td></tr>
  <tr><th>Descrição</th><td>Engenheiros de Produto de Software</td></tr>
  <tr><th>Tipo</th><td>Graduandos de Engenharia de Software na Universidade de Brasília, matriculados na disciplina de Engenharia de Produto de Software.</td></tr>
  <tr><th>Responsabilidades</th><td>Planejar o projeto, programar os recursos definidos do projeto e gerir a equipe de desenvolvedores. A equipe é composta pelo Product Owner, Scrum Master, DevOps e Arquiteto que desempenham os papéis de, respectivamente, compreender o mercado e vender a idéia ao investidor, guiar e facilitar as tarefas realizadas pela equipe, configurar o ambiente de desenvolvimento do projeto e estudar formas de implementação do sistema por completo.</td></tr>
  <tr><th>Critérios de Sucesso</th><td>Entregar a aplicação no tempo estimado, vender a idéia da aplicação aos investidores e aumentar a experiência na área de desenvolvimento de software e gestão de projetos.</td></tr>
  <tr><th>Envolvimento</th><td>Alto</td></tr>
  <tr><th>Comentários / Problemas</th><td>-</td></tr>
</table>

### 3.4 Perfis dos Usuários

#### 3.4.1 Administrador

<table>
  <tr><th>Descrição</th><td>Funcionário que faz parte da administração da área financeira ou de confiança  da empresa.</td></tr>
  <tr><th>Tipo</th><td>Usuário avançado</td></tr>
  <tr><th>Responsabilidades</th><td>Conhecer a aplicação de modo que possa organizar os PDFs presentes na aplicação, gerenciar gastos no sistema, adicionar novas empresas ao sistema e realizar o cadastro de novos usuários.</td></tr>
  <tr><th>Critérios de Sucesso</th><td>Receber um sistema capaz de automatizar tarefas repetitivas que envolvem notas fiscais.</td></tr>
  <tr><th>Envolvimento</th><td>Usuário final do sistema</td></tr>
  <tr><th>Comentários / Problemas</th><td>-</td></tr>
</table>

#### 3.4.2 Funcionário

<table>
  <tr><th>Descrição</th><td>Funcionários que fazem parte do setor financeiro.</td></tr>
  <tr><th>Tipo</th><td>Usuário comum</td></tr>
  <tr><th>Responsabilidades</th><td>Conhecer a aplicação de modo que possa organizar os PDFs presentes na aplicação e gerenciar gastos no sistema.</td></tr>
  <tr><th>Critérios de Sucesso</th><td>Receber um sistema capaz de automatizar tarefas repetitivas que envolvem notas fiscais.</td></tr>
  <tr><th>Envolvimento</th><td>Usuário final do sistema</td></tr>
  <tr><th>Comentários / Problemas</th><td>-</td></tr>
</table>

### 3.5 Principais Necessidades dos Usuários ou dos Envolvidos

| Necessidade | Prioridade | Preocupações | Solução Atual | Soluções Propostas |
|:---:|:---:|:---:|:---:|:---:|
| Agilidade e automatização na análise e armazenamento de notas fiscais. | Alta | Falta de agilidade na análise das notas fiscais e possíveis erros humanos. | Verificação manual das notas fiscais | Realizar a leitura da nota fiscal com sua divisão por blocos na qual as mesmas são adicionadas para serem lidas de forma automática. |
| Gerar relatórios com base nas notas fiscais recebidas. | Alta | Possíveis erros humanos na hora da elaboração do relatório | Feito de forma manual. | De acordo com a leitura feita nas notas fiscais, a aplicação irá gerar análises conforme a necessidade do usuário. |

### 3.6 Alternativas e Concorrência

#### 3.6.1 Noov
É uma plataforma web gratuito onde é possível realizar o armazenamento de NFes que garante o backup seguro de suas notas na nuvem tendo também a opção de envio ou recebimento de notas fiscais de forma automática. O Noov permite também compartilhar as notas fiscais da empresa com seus clientes, parceiros e contadores. Esse portal possui uma API voltada a desenvolvedores com o intuito de desenvolverem novos aplicativos e colaborarem com a plataforma Noov. Essa plataforma não lê notas fiscais em PDF e não há análise dos gastos financeiros.

![Noov](https://uploaddeimagens.com.br/images/001/604/543/original/Noov.png?1536550429)


#### 3.6.2 Arquivei
Desenvolvido e mantido por uma startup constituída por alunos e ex-alunos da Universidade de São Paulo, o Arquivei é uma plataforma web paga que tem como objetivo o acesso fácil aos documentos fiscais da empresa. A plataforma é conectado à Secretaria da Fazenda e baixa automaticamente todas as NFes e CTes emitidas para o CNPJ da empresa, armazenando-as no painel de gestão de notas da plataforma. Todas informações presentes na plataforma se tornam gráficos para melhor visualização do usuário. O Arquivei possui três planos de contratação com taxas mensais: o primeiro, Plano Starter, no valor de R$ 29,90; o segundo com o nome de Plano Controle no valor de R$ 49,90; e o terceiro plano, intitulado Plano Business, possuindo o valor de R$ 89,90. Essa plataforma não lê notas fiscais em PDF e não há uma gama de tipos de análises.

![Arquivei](https://uploaddeimagens.com.br/images/001/604/545/original/Arquivei.png?1536550547)


***
## 4. Visão Geral do Produto
***

### 4.1 Perspectiva do Produto

O PDF2CASH irá sistematizar o processo de leitura e transformação de NFes de tal forma que diretores e funcionários da empresa tenham o controle sobre seus gastos. O produto fornecerá aos usuários as informações necessárias para melhor gestão da financeira. Tais informações contemplam categoria de gastos, valores unitários, valores totais, análise de dados, margem de gastos, histórico de gastos. Assim, têm-se como expectativa facilitar e agilizar o processo de controle fiscal, além de ampliar os lucros pelo fato de ter-se um controle automatizado dos gastos.

### 4.2 Resumo dos Recursos

<table>

  <tr><th>Benefício para o Cliente</th><th>Recursos de Suporte</td></tr>
  <tr><td>Agilidade no processamento dos dados sem a necessidade da criação de planilhas.</th><td>Uma base de conhecimentos ajuda o pessoal de suporte a identificar rapidamente ações corretivas e soluções conhecidas.</td></tr>
  <tr><td>O usuário poderá descobrir em que ou onde é o seu maior gasto, podendo assim melhorar o seu planejamento financeiro.</th><td>Os problemas são relacionados como itens únicos, classificados e monitorados ao longo de todo o processo de resolução. São emitidas notificações automáticas para os problemas que têm seus prazos expirados.
  </td></tr>
  <tr><td>A margem de gastos calculada dará ao usuário uma noção do quanto será o gasto estimado do mês, semana ou ano.
  </th><td>Os relatórios de tendências e de distribuição permitem revisões de nível superior do status dos problemas.
  </td></tr>
  <tr><td>
  Os clientes têm autonomia para resolver seus problemas, o que reduz os custos de suporte e melhora o tempo de resposta.
  </td></th>
  </th><td>Um servidor de duplicação permite que as informações atuais do banco de dados sejam compartilhadas pela empresa.
  </td></tr>
</table>

### 4.3 Custos e Preços

### 4.4 Licenciamento e Instalação

Será necessária a instalação do software pois o mesmo será uma aplicação Desktop.
O licenciamento do produto será do tipo MIT(software livre). No caso é concedida permissão, gratuitamente, a qualquer pessoa que obtenha uma cópia deste software e dos arquivos de documentação associados, para negociar o Software sem restrições, incluindo, sem limitação, os direitos de uso, cópia, modificação e fusão, publicar, distribuir, sublicenciar e/ou vender cópias do Software, além de permitir que as pessoas a quem o Software é fornecido o façam.
***
## 5. Recursos do Produto
***

### Legenda de Prioridades dos Requisitos:

<table>
  <tr><th>Prioridade</th><th>Caracteristica</td></tr>
  <tr><td>Alta</th><td>Requisito fundamental para o sistema. </td></tr>
  <tr><td>Intermediaria</th><td>Requisito importante, mas não é fundamental para o funcionamento do sistema.</td></tr>
  <tr><td>Baixa</th><td>Requisito não fundamental e pouco usado no sistema.</td></tr>

</table>


| Identificador| Nome | Descrição | Prioridade |
|:----:|:---------:|:-----------------:|:--------|
| RF1 | Geração de gráficos  |O sistema de maneira automática deve gerar gráficos baseados nos gastos condizente nas notas fiscais. | Alta |
| RF2 | Arquivação de notas fiscais | O sistema deve arquivar de maneira automática, ou não, as notas fiscais que forem inseridas no programa. | Alta |
| RF3 | Gerenciamento de funcionario | O sistema deve possuir uma maneira de gerência de funcionarios. | Media |
| RF4 | Consulta no histórico de gastos | O sistema deve possuir uma maneira de gerar informações cronológicas de gastos com as notas fiscais. | Media
| RF5 | Criar contas | O sistema deve possuir uma maneira que possibilite o usuário criar e administrar diversas contas. | Alta
| RF6 | Processo de autenticação | O sistema deve possuir uma maneira que o usuário possa fazer o processo de autenticação. Login e logout. | Media
| RF7 | Deletar notas fiscais | O sistema deve possuir uma maneira que o usuário possa deletar as notas fiscais cadastradas no banco de dados. | Media

***
## 6. Restrições
***
* O PDF deverá ser nativo, sendo assim, um PDF “original” com texto selecionável (sem ser um PDF escaneado).
* O sistema funcionará apenas para notas fiscais.
* Notas fiscais deverão seguir um determinado padrão, para ser reconhecido os valores pelo parser e lexer.
* Apenas o Administrador poderá gerenciar os outros usuários, como a criação das contas dos funcionários.
* Conhecimento básico em Português e Inglês.

***
## 7. Intervalos de Qualidade
***

### 7.1   Requisitos de Sistema
* O sistema consiste em uma aplicação desktop na qual o acesso a rede será necessário apenas para instalação e atualizacão do mesmo.
* Deve ser possível instalar a aplicação desktop em sistemas operacionais de distribuição Linux.

### 7.2   Requisitos de Desempenho
* O PARSER deve ser capaz de ler e converter em dados as informações contidas nas notas fiscais em menos de um segundo.
* Os gráficos de dados das notas fiscais devem ser atualizados assim que a pagina onde os mesmos se encontram seja novamente carregada.
* O sistema deverá autenticar rapidamente todo usuário que deseje utilizar o software.

### 7.3   Requisitos de Design
* O sistema deve ter uma interface organizada e intuitiva suficiente para o uso adequado, tendo ícones, simbolos e cores indicadores que possam diferenciar cada funcionalidade.

### 7.4   Requisitos de Confiabilidade      
* O sistema deve calcular com precisão os valores de cada item na nota fiscal.
* O sistema deve poder se recuperar de falhas que possam ocorrer durante a sua utilização.

### 7.5   Requisitos de Arquitetura
* O sistema deve possuir uma arquitetura orientada a micro serviços.
* O sistema deve seguir a modelagem definida pelo arquiteto da equipe.

### 7.6   Requisitos de Usabilidade
* A interface do sistema deve ser responsivo de acordo com o tamanho de tela do usuário.
* A interface do sistema deve instruir o usuário no preenchimento de campos de formulários.
* O sistema deve exibir notificações caso tenha erro ou sucesso no preenchimento do formulário.

### 7.7   Requisitos de Suportabilidade
* Deve ser possível fazer a instalação do sistema na máquina do usuário para a execução do mesmo.
* O sistema deve seguir o padrão de codificação criado pelo integrate devops da equipe.

### 7.8   Requisitos de Segurança
* O sistema deve armazenar e administrar os dados dos funcionários de forma a garantir a privacidade dos mesmos.
* O sistema deve impedir o acesso de pessoas não autorizadas.
* O sistema deve possuir validação para cada dado inserido no banco de dados.
