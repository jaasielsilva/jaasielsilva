# Loja de Veículos - Sistema de Cadastro

## Descrição

Este projeto é um sistema de cadastro de clientes para uma loja de veículos, desenvolvido em Java com Swing para a interface gráfica. O sistema permite a entrada de dados de clientes e armazena essas informações em um banco de dados MySQL. Além disso, o projeto utiliza o JasperStudio para geração de relatórios.

## Funcionalidades

- Cadastro de clientes
- Formatação automática de números de telefone
- Armazenamento de dados em banco de dados MySQL
- Geração de relatórios com JasperStudio

## Requisitos

- JDK 8 ou superior
- MySQL Server
- JasperStudio
- IDE de sua preferência (Eclipse, IntelliJ, NetBeans, etc.)

## Dependências

### MySQL

- **Driver JDBC do MySQL:** Necessário para a conexão do projeto Java com o banco de dados MySQL.

### JasperStudio

- **Bibliotecas do JasperReports:** Utilizadas para criação e exibição de relatórios a partir de dados armazenados no banco de dados.
- ![JasperStudio](https://upload.wikimedia.org/wikipedia/commons/thumb/0/0d/Jaspersoft_logo.png/150px-Jaspersoft_logo.png)

## Instalação

### Configuração do Ambiente

1. **Instale o JDK:**
    - Baixe e instale o JDK 8 ou superior a partir do [site oficial da Oracle](https://www.oracle.com/java/technologies/javase-downloads.html).

2. **Configure o MySQL:**
    - Baixe e instale o MySQL Server a partir do [site oficial do MySQL](https://dev.mysql.com/downloads/installer/).
    - Crie um banco de dados para armazenar os dados dos clientes.
    - Exemplo de criação de banco de dados:
      ```sql
      CREATE DATABASE loja_veiculos;
      ```
    - Exemplo de criação de tabela:
      ```sql
      USE loja_veiculos;
      CREATE TABLE clientes (
          id INT AUTO_INCREMENT PRIMARY KEY,
          nome VARCHAR(100),
          telefone VARCHAR(20),
          email VARCHAR(100)
      );
      ```

3. **Instale o JasperStudio:**
    - Baixe e instale o JasperStudio a partir do [site oficial do Jaspersoft](https://community.jaspersoft.com/project/jaspersoft-studio).

### Adicionar Dependências ao Projeto

1. **Adicione o driver JDBC do MySQL:**
    - Baixe o arquivo `mysql-connector-java.jar` do [repositório oficial](https://dev.mysql.com/downloads/connector/j/).
    - Adicione o arquivo JAR ao build path do seu projeto na sua IDE.

2. **Adicione as bibliotecas do JasperReports:**
    - Baixe as bibliotecas necessárias a partir do [site oficial do Jaspersoft](https://community.jaspersoft.com/project/jasperreports-library).
    - Inclua as bibliotecas no build path do seu projeto na sua IDE.

## Uso

### Executando o Projeto

1. Abra o projeto na sua IDE.
2. Compile e execute o projeto.
3. Utilize a interface gráfica para cadastrar clientes e gerar relatórios.

### Configurando a Conexão com o Banco de Dados

- Certifique-se de que os detalhes de conexão do MySQL estejam corretos no seu código. Abaixo está um exemplo de configuração de conexão:

```java
import java.sql.Connection;
import java.sql.DriverManager;
import java.sql.SQLException;

public class DatabaseConnection {
    private static final String URL = "jdbc:mysql://localhost:3306/loja_veiculos";
    private static final String USER = "root";
    private static final String PASSWORD = "sua_senha";

    public static Connection getConnection() throws SQLException {
        return DriverManager.getConnection(URL, USER, PASSWORD);
    }
}