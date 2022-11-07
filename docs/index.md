# Documentação Ponto eletrônico Compliance 


##Sobre a documentação

&ensp; Essa é uma documentação mais voltada em descrever os principais processos que envolvem o aplicativo. Ou seja, não é uma documentação detalhada que contém uma relação completa de classes, atributos, metodos, etc. Esses elementos serão abordados de forma pontual conforme as explicações dos processos forem citando as classes, metodos, etc; Mesmo assim, não serão abordados na sua totalidade, de forma que serão citados apenas os elementos principais que são cruciais para o entendimento do processo. 


##Linha do tempo 

&ensp; No projeto foram implementadas algumas abordagens que a primeira vista parecem complicações, mas foram decisões tomadas dentro de um determinado contexto levando em consideração questões como prazo de entrega, força de trabalho disponível, etc.  
&ensp; Por conta disso, será representada uma linha do tempo do projeto, antes de entrar nos detalhes da documentação. A linha do tempo facilita o entedimento da organização atual do projeto. 

**Linha do tempo:** 

### 1. Projeto pronto, aguardando lançamento. 
Neste ponto, existia um projeto ja pronto porém que ainda não havia sido lançado em produção. O projeto ficou de lado enquanto aguardava lançamento. 

### 2. Inicio do lançamento em produção.   <br/>
O aplicativo começou a ser utilizado pelos clientes. Nessa utilização real, começaram a aparecer alguns comportamentos indesejados, por exemplo: Batida com horário errado; Batidas duplicadas, e alguns outros. <br/>
No primeiro momento, as correções foram realizadas diretamente no código ja existente, focando especificamente a correção do problema, sem envolver refatoração. 

### 3. Refatoração / Versão 2.0  <br/>
Trabalhar direto no código ja existente não se mostrou produtivo, devido a alguns fatores. Por conta disso, o desenvolvedor responsável no momento optou por iniciar uma revisão geral do aplicatvo, algo além de uma refatoração.  <br/>
 Nessa revisão, a regra de negócios do app seria elaborada do zero, melhorando aspectos como tipagem, implementação de design patterns, organização do código, etc. <br/>
 Mas o tempo era uma preocupação, então o projeto não poderia parar e aguardar ser refeito totalmente do zero. Por conta disso, foi decicido ir refazendo o aplicativo por partes, de forma que algumas funcionalidedades/telas continuariam sendo da versão anterior, enquanto outros recursos seriam feitos do zero. Para fazer isso na prática, o aplicativo foi quebrado em dois projetos Flutter, um deles sendo o projeto ja existente, e o outro onde seriam desenvolvidas as telas/funcionalidades do zero, da seguinte forma: <br/> 

#### PTEM - CORE 

Projeto que ja existia, onde foram realizadas as configurações nativa de compilação. Esse projeto é o "core", ou seja, é ele que é compilado, de forma que o outro projeto é importado dentro desse projeto principal.   <br/> 
Em termos de funcionalidades, recursos e telas, esse projeto tem no momento os seguintes elementos: <br/> 
- Inicialização do Aplicativo: Toda a lógica responsável por inicializar o app, ou seja, definir rota inicial (verificando se esta autenticado), recuperar alguns dados persistidos localmente, etc. <br/>
- Login/Cadastro: Telas de login e cadastro. <br/>
- Telas secundárias (telas de relatórios, por ex: batidas por data, etc) <br/>

#### PTEM 2.0 

   **PTEM 2.0 - ** Projeto onde estão sendo desenvolvidos os recursos do zero, visando melhoria. Esse projeto é importado dentro do PTEM, como se fosse um package. 
    Em termos de funcionalidades, recursos e telas, esse projeto tem no momento os seguintes elementos: <br/> 







