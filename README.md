# simple-api-csharp

Api rest com swagger

## Instalação

### Configuração do Docker Local com Liquibase

Siga estas etapas para configurar o ambiente de desenvolvimento local usando Docker e Liquibase:

#### Pré-requisitos

Antes de começar, certifique-se de que você tenha os seguintes pré-requisitos instalados em sua máquina:

- Rancher Desktop: [Instalação do Rancher](https://docs.rancherdesktop.io/getting-started/installation/)
- Docker Compose: [Instalação do Docker Compose](https://docs.docker.com/compose/install/)
- Java (JRE ou JDK) versão X ou superior: [Instalação do Java](https://www.oracle.com/java/technologies/javase-downloads.html)
- Liquibase: [Instalação do Liquibase](https://www.liquibase.org/get-started)

#### Passos de Configuração

1. Clone este repositório para a sua máquina local:

   ```shell
   git clone https://github.com/lorrayneantonielle/simple-api-csharp.git

2. Acesse o diretório do projeto:
   ```shell
   cd simple-api-csharp

3. Na raiz do projeto, configure o arquivo docker-compose.yml conforme necessário para sua aplicação e banco de dados. 

4. Execute o seguinte comando para iniciar os contêineres Docker:
   ```shell
    docker-compose -f docker-compose.yml -p liquibase-simple-api --verbose up --force-recreate  

5. Para ver os contêineres funcionando, basta no terminal, inserir o comando
   ```shell
    docker ps 
   
#### Verifique os log
Caso você encontre erros ao subir os contêineres Docker, verifique os logs dos contêineres para obter informações detalhadas sobre qualquer erro.:

1. Use o comando:
   ```shell
    docker-compose -f docker-compose.yml -p liquibase-simple-api logs 

#### Usos do Liquibase
Para criar novas migrações de banco de dados, você pode usar os comandos Liquibase apropriados. Consulte a [documentação do liquibase](https://docs.liquibase.com/home.html?_ga=2.142770608.420775302.1694451423-1990558979.1693945692) para mais informações.

#### Encerrando os Contêineres
1. Execute o seguinte comando para encerrar os contêineres Docker:
   ```shell
    docker-compose -f docker-compose.yml -p liquibase-simple-api --verbose down
## Uso

Sinta-se livre para dar exemplos, e mostre o resultado esperado, se puder. É útil ter descrito o menor exemplo de uso que você pode demonstrar, enquanto fornece links para exemplos mais sofisticados se eles forem muito longos para incluir razoavelmente no README.

## Suporte

Diga às pessoas onde elas podem ir para obter ajuda. Pode ser qualquer combinação nome de pessoas responsáveis, uma sala de bate-papo, um endereço de e-mail, etc.

## Contribuindo

Para pessoas que possam precsiar de fazer alterações neste projeto, é útil ter alguma documentação sobre como começar. Talvez haja um script que eles devam executar ou algumas variáveis de ambiente que precisam definir. Torne essas etapas explícitas. Essas instruções também podem ser úteis para o seu futuro eu.

Você pode também documentar comandos para formatar o código ou para rodar testes. Essas etapas ajudam a garantir alta qualidade de código e reduzem a probabilidade de que as alterações quebrem algo inadvertidamente.
