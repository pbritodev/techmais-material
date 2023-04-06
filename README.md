# Perguntas Jorge Felippe para Miriam
1 - Quem você quer que abra os chamados? Vai ter um setor específico? Seria a equipe de TI? Ou os gerentes de cada setor?

2 - Quando o chamado for aberto, o cliente vai receber alguma notificação de acompanhamento? Ou ele tem que entrar no app par verificar se o chamado já foi concluido?

3 - O sistema irá funcionar 24hrs? Ou essa função dependeria do tipo de cliente?


# Requisitos do projeto (5W2H):
## Quem?
 -Empresa Microméros que atua no setor industrial e utiliza IOT para a tomada de decisões de seus clientes. A empresa fornece a infraestrutura, a instalação e a manutenção dos sensores, e ainda fornece relatorios com os dados coletados, por meio de gráficos, telas de payback e insights. A Microméros atua no eixo industrial, atendendo fábricas, transportadoras, etc. 

-Equipe de tecnologia. Restrito. Login, registro e usuários. Permissões personalizadas. Cargo de administrador é o único com a permissão de registro de novos 		    usuários.
- O sistema é para os setores de tecnologia, setor comercial e setor de operações.

## Quando?
	O projeto será desenvolvido no 1º semestre de 2023. 
    
## O que?
	A empresa busca um sistema web para controle de chamados. O sistema deve:
- ter login e senha (somente o administrador pode criar novos usuários e gerencias as permissões de 0);
- controlar o acesso dos usuários;
- classificar os chamados por meio de uma divisão entre os setores e subdivisões por hierarquia de urgência;
- controlar diariamente a quantidade de chamados abertas e fechados/concluidos nos diferentes departamentos; 
- classificar os chamados em "Pendentes", "Abertos" ou "Resolvidos";
- informar os dados para o gerente de operação em tempo real ( criação de um relatorio com informaçoes diárias e dicas especializadas, tais como: número de soluções por dia, relatorios e análises detalhadas, eventos e log de eventos, para gestão de desempenho operacional; Gestão de métricas e desempenho. 
- SLA (Acordo de Nível de Serviço) de acordo com as prioridades dos chamados (ex: queda de um servidor - chamado urgente). Caso, um chamado expire, o mesmo deve ser duplicado no card de pendente e expirado, pq mesmo assim deve ter uma solução o quanto antes

	Os dados utilizados para o desenvolvimento do sistema serão fícticios. Além das características descritas anteriormente, o sistema também precisa: 
- ser Interativo, prático e eficiente;
- ter Responsividade, ou seja, ser adaptável com possibilidade de acesso via mobile.
- guardar informações em Logs.
  
## Onde?
  	O sistema deve funcionar tanto em computadores como em dispositivos móveis. 
    
## Por que?
	O sistema antigo utilizado pela empresa possui algumas falhas e não estava suprindo as necessidades operacionais da empresa. A principais críticas do antigo sistemas são: 
  - O sistema antigo não é orientado a chamados;
  - Há dificuldade em guardar informações dos chamados (logs) e os mesmos se perdem como tempo;
  - Não há informações relevantes para os analistas;
  - Os funcionários precisam se reunir presencialmente para a analise dos dados, pois os dados que aparecem no sistema são de dificil interpretação  

 ## Quanto?
 	O projeto não possui custo inicial monetário, apenas tempo.
    
## Como?
	O sistema será construído com base em conceitos de Design Thinking e metodologias ágeis. Também serão utilizadas ferramentas de codificação de aplicação com uso de framework JavaScript (Angular, React, Vue.js ou similar), em ambiente de desenvolvimento integrado ou editor de texto com complementação de código (Visual Studio Code, Atom, Sublime ou similar), utilização de dados provenientes de API web, integração com mídias e imagens, implementação de design de interface adaptável a diferentes tamanhos de tela (proporcional, responsivo, media queries, mobile first).
	
## Lista de Requisitos Funcionais em tópicos:

### 1 - Login e cadastro
  -O sistema deve permitir que o usuário faça login para acessar suas funcionalidades; <br />
  -O sistema deve permitir que o administrador cadastre novos usuários, defina a senha e o setor do usuário; <br />
  -O sistema deve permitir que o administrador defina a área do usuário (Comercial, TI e operações), suas permissões e a senha desejada; <br />
  -O sistema deve permitir a criação de um usuário-cliente, para que o mesmo possa acompanhar o andamento do seu chamado; <br />

### 2 - Dashboard 
  -O sistema deve exibir um dashboard para gerenciamento de chamados; <br />
  -O sistema deve permitir que o usuário cadastrado crie chamados, defina nome, prazo (SLA), área responsável e uma caixa de texto para a descrição do problema; <br />
  -O sistema deve possuir um dashboard para cada departamento e um geral, que exibe todos os chamados. Apenas o administrador pode visualizar o dashboard geral. Os usuários com permissão de área específica terão acesso apenas ao dashboard do seu setor; <br />
  -O sistema deve possuir uma área específica para o setor de TI, com chamados internos do setor; <br />
  -O sistema deve verificar as permissões do usuário e exibir apenas o chamado do seu setor; <br />

### 3 - SLA
  -O sistema deve definir o SLA do cliente que solicitou a abertura do chamado. O prazo de atendimento será o acordado no SLA (Acordo de Nível de Serviço); <br />
  -O sistema deve permitir que os usuários definam o tipo do chamado, o prazo e exibir o usuário que abriu; <br />

### 4 - Chamados 
  #### O sistema deve exibir chamados com:
      -Sua descrição;
      -SLA;
      -Categoria (área);
      -Data de abertura/fechamento;
      -Usuário responsável pela abertura;
      -TAG de análise, em andamento ou resolvido.

### 5 - Métricas e qualidade
  -O sistema deve exibir quantos chamados foram abertos e quantos foram finalizados no dia; <br />
  -O sistema deve exibir, no fechamento de um chamado, uma pesquisa de satisfação para o atendimento e para a plataforma; <br />

## Lista de requisitos não funcionais em tópicos:
  - Implementar e definir o SLA (Acordo de Nível de Serviço) de cada cliente no sistema;<br />
  - O sistema deve ser desenvolvido com a tecnologia ReactJS;<br />
  - O sistema deve armazenar seus dados em um banco de dados MariaDB;<br />
  - O sistema deve ser feito para WEB e de forma responsiva, ou seja, multi-device;<br />
  - O sistema deve ser confiável e ter alta disponibilidade;<br />
  - O sistema deve ter uma interface fácil de usar e intuitiva;<br />
  - O sistema deve ser fácil de manter e atualizar;<br />
  - O sistema deve ser seguro e proteger as informações do usuário;<br />
  - O sistema deve ficar disponível 24h, ser escalável e responsivo;<br />
 - O sistema deve ser capaz de lidar com 7 usuários simultâneos, usando diferentes funcionalidades;<br />


