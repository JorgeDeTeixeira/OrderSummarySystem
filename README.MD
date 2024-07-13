# Order Management System

Este é um sistema simples de gerenciamento de pedidos escrito em Java. O sistema permite que você crie clientes, faça pedidos e adicione itens a esses pedidos. O sistema, então, exibe um resumo do pedido.

## Estrutura do Projeto

O projeto está organizado da seguinte maneira:

.
##### ├── src
##### │ ├── application
##### │ │ └── Main.java
##### │ ├── entities
##### │ │ ├── Client.java
##### │ │ ├── Order.java
##### │ │ ├── OrderItem.java
##### │ │ └── Product.java
##### │ └── entities/enums
##### │ └── OrderStatus.java
##### └── README.md


### Pacote `application`

- **Main.java**: Contém o método `main` que executa o programa. Responsável por coletar dados do usuário e exibir o resumo do pedido.

### Pacote `entities`

- **Client.java**: Representa um cliente com nome, e-mail e data de nascimento.
- **Order.java**: Representa um pedido com data, status, cliente e itens.
- **OrderItem.java**: Representa um item do pedido com quantidade, preço e produto.
- **Product.java**: Representa um produto com nome e preço.

### Pacote `entities.enums`

- **OrderStatus.java**: Enumeração que define os possíveis status de um pedido.

## Funcionamento do Programa

O programa realiza as seguintes etapas:

1. Solicita os dados do cliente (nome, e-mail e data de nascimento).
2. Solicita os dados do pedido (status).
3. Solicita os dados dos itens do pedido (nome do produto, preço e quantidade).
4. Exibe um resumo do pedido, incluindo o total.

## Exemplo de Uso

Ao executar o programa, ele solicitará entradas do usuário conforme o exemplo abaixo:

###### Enter client data:
###### Name: John Doe
###### Email: john.doe@example.com
###### Birth date (DD/MM/YYYY): 15/05/1990
###### 
###### Enter order data:
###### Status: PROCESSING
###### 
###### How many items to this order? 2
###### Enter #1 item data:
###### Product name: Laptop
###### Product price: 1200.00
###### Quantity: 1
###### 
###### Enter #2 item data:
###### Product name: Mouse
###### Product price: 40.00
###### Quantity: 2
###### 
###### ORDER SUMMARY:
###### Order moment: 13/07/2024 15:30:45
###### Order status: PROCESSING
###### Client: John Doe (15/05/1990) - john.doe@example.com
###### Order items:
###### Laptop, $1200.00, Quantity: 1, Subtotal: $1200.00
###### Mouse, $40.00, Quantity: 2, Subtotal: $80.00
###### Total price: $1280.00


## Como Executar o Projeto

### Pré-requisitos

- Java Development Kit (JDK) 8 ou superior.
- Um IDE de sua escolha (Eclipse, IntelliJ, etc.) ou um editor de texto (VS Code, Sublime, etc.).

### Passos para Execução

1. Clone o repositório para sua máquina local:

    ```sh
    git clone https://github.com/seu-usuario/order-management-system.git
    ```

2. Importe o projeto em sua IDE ou abra os arquivos em seu editor de texto.

3. Compile e execute a classe `Main` localizada no pacote `application`.

## Melhorias Futuras

- Adicionar validações de entrada do usuário.
- Implementar uma interface gráfica para facilitar a interação do usuário.
- Integrar com um banco de dados para persistência de dados.

## Contribuição

Se você deseja contribuir com este projeto, por favor, siga as etapas abaixo:

1. Fork o repositório.
2. Crie uma nova branch (`git checkout -b feature/nova-funcionalidade`).
3. Commit suas alterações (`git commit -m 'Adiciona nova funcionalidade'`).
4. Faça o push para a branch (`git push origin feature/nova-funcionalidade`).
5. Abra um Pull Request.

## Licença

Este projeto está licenciado sob a Licença MIT. Veja o arquivo [LICENSE](LICENSE) para mais detalhes.

