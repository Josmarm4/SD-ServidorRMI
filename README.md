# RMI Server/Client

Este é um exemplo básico de implementação de comunicação entre processos utilizando Java RMI (Remote Method Invocation). O projeto consiste em um servidor (`HelloServer`) que fornece um método remoto `sayHello()`, e um cliente (`HelloCliente`) que invoca esse método para obter uma resposta.

## Requisitos

Antes de executar o projeto, certifique-se de que tem o **Java Development Kit (JDK)** instalado na sua máquina. O projeto foi desenvolvido usando o **OpenJDK 21.0.4**.

- Java 8 ou superior
- `rmiregistry` disponível no seu ambiente de desenvolvimento

## Estrutura do Projeto

- **HelloServer.java**: Contém a implementação do servidor RMI que disponibiliza o método remoto.
- **HelloCliente.java**: Contém o código do cliente RMI que chama o método remoto do servidor.
- **README.md**: Este arquivo.

## Passos para Execução

Siga os passos abaixo para compilar e executar o servidor e o cliente RMI.

### 1. Compile os arquivos Java

Abra o terminal e navegue até o diretório do projeto. Em seguida, execute o comando para compilar os arquivos Java:

```bash
javac *.java
```
2. Inicie o RMI Registry
```bash
rmiregistry &
```
3. Execute o Servidor
```bash
java HelloServer
```
4. Execute o Cliente
```bash
java HelloCliente localhost
```