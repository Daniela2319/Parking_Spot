# Parking_Spot API REST com Spring Boot

Spring Boot é um framework do ecossistema Spring para construção de aplicativos em Java. Ele facilita a criação de aplicativos robustos, escaláveis e fáceis de manter, além de oferecer uma ampla gama de recursos e funcionalidades, tais como:

•	Configuração automática: o Spring Boot detecta as bibliotecas e dependências presentes no classpath e configura automaticamente a aplicação.

•	Servidor embutido: o Spring Boot inclui um servidor web embutido, como o Tomcat, o Jetty ou o Undertow, permitindo que o aplicativo seja executado diretamente a partir do JAR ou WAR gerado.

•	Starter Packs: o Spring Boot oferece pacotes de inicialização, chamados Starter Packs, que contêm as dependências necessárias para integrar com diferentes tecnologias e serviços, como banco de dados, segurança, serviços em nuvem, etc.

•	Atualizações de versão simplificadas: o Spring Boot gerencia as dependências e atualizações de versão automaticamente, o que torna a atualização de versão de bibliotecas e dependências muito mais fácil.


![image](https://user-images.githubusercontent.com/106537496/235810774-48ad8b80-2e69-4075-a711-404195d79b08.png)



 ##  Tecnologias

Esse projeto foi desenvolvidos com as seguintes tecnologias:
- Spring Initializ: Dependencias Web, DataJPA, Validation, Postgresql
- Banco Dados Postgresql
- IDE 
- Github

## API REST 

É uma aplicação cliente/servidor que envia e recebe dados através do protocolo HTTP utilizando de padrões de comunicação com XML e JSON.
Neste projeto foi desenvolvido uma API REST para vagas de estacionamento de apartamentos. Assim é feito o cadastro do responsavel da vaga, que tem direito a uma vaga
de estacionamento.

## Modelo

Primeiro criado o modelo que será a representação do recurso na URI da API Parking-Spot: 

{
    "parkingSpotNumber": "115C",
    "licensePlateCar": "IRF8567",
    "brandCar": "corola",
    "modelCar": "toyota",
    "colorCar": "prata",
    "responsibleName": "Frank Joao",
    "apartment": "115",
    "block": "C"
}

## Repository

ParkingSpotRepository onde extende JPARepository do Spring Data para utilizar os métodos já prontos para transações com o banco de dados.
Assim, métodos com finAll(), findById(id), save(), delete(), entre outros.

## Service

Criado a classe de Serviço para os métodos ser utilizado no controller.

## Controller

Criando o controle pra construção da API REST onde será implementado os endpoint da aplicação.

## Métodos

POST - Para criar uma nova vaga de estacionamento.

GET ALL - Retorna URI/Parking-Spot

GET ONE - Retorna URI/Pariking-Spot/{id} 

PUT - Atualiza as informações da vaga de estacionamento caso mude de carro ou apartamento

DELETE - Apaga caso ocorreu algum erro de informação


Projeto foi denvolvido Michele Brito estou utilizando para estudo na API REST com Spring Boot.

