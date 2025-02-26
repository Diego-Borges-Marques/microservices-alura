# Projeto: Sistema de Gerenciamento de Pedidos com Microserviços

# Descrição
Este projeto tem como objetivo desenvolver um Sistema de Gerenciamento de Pedidos utilizando a arquitetura de microserviços. A arquitetura de microserviços permite a criação de aplicações modulares e escaláveis, onde cada funcionalidade do sistema é implementada como um serviço independente. Isso facilita a manutenção, a escalabilidade e a implantação contínua.

# Conceitos Básicos
Microserviços: Arquitetura onde uma aplicação é dividida em pequenos serviços autônomos que se comunicam entre si, geralmente por meio de APIs RESTful.

# Service Discovery (Descoberta de Serviços): 
Processo pelo qual os microserviços encontram uns aos outros na rede. Ele garante que os serviços possam se comunicar dinamicamente, sem depender de configurações estáticas.

Service Register (Registro de Serviços):
# Um repositório onde os microserviços se registram com suas informações de rede, como endereços IP e portas, para que possam ser descobertos por outros serviços.

# Ferramentas Utilizadas

# Eureka:

Função: É um serviço de descoberta e registro de serviços desenvolvido pela Netflix.

Uso no Projeto: Os microserviços se registram no Eureka Server, que mantém um catálogo dos serviços disponíveis e facilita a descoberta dinâmica.

# Gateway:

Função: Atua como um ponto de entrada único para todas as solicitações externas ao sistema.

Uso no Projeto: O API Gateway roteia as solicitações dos clientes para os microserviços apropriados, aplicando políticas de segurança, autenticação e agregação de dados.

# OpenFeign:

Função: É um cliente HTTP declarativo para facilitar a comunicação entre microserviços.

Uso no Projeto: OpenFeign permite que os microserviços consumam APIs de outros serviços de maneira simplificada, utilizando anotações para definir as interfaces e métodos de comunicação.

Benefícios do Projeto
Escalabilidade: Cada microserviço pode ser escalado independentemente com base na demanda.

Manutenibilidade: Alterações e atualizações podem ser feitas em serviços individuais sem impactar todo o sistema.

Desenvolvimento Independente: As equipes de desenvolvimento podem trabalhar em diferentes serviços de forma autônoma e em paralelo.

# Conclusão
Este projeto exemplifica como a arquitetura de microserviços, aliada a ferramentas poderosas como Eureka, Gateway e OpenFeign, pode ser utilizada para criar sistemas robustos, escaláveis e de fácil manutenção. Através da implementação de conceitos básicos como service discovery e service register, os microserviços podem se comunicar de maneira eficiente e dinâmica.
