
# RPC_RabbitMQ

## 1) Passo:
- Instalando o **pika**:
  ```bash
  pip install pika --break-system-packages
  ```

## 2) Rodar o Docker do RabbitMQ (mais fácil):
- Para rodar a última versão do RabbitMQ com o plugin de gerenciamento:
  ```bash
  docker run -it --rm --name rabbitmq -p 5672:5672 -p 15672:15672 rabbitmq:4.0-management
  ```

## 3) Verificar e acessar o RabbitMQ no localhost:
- Acesse o RabbitMQ através do navegador:
  [http://localhost:15672/](http://localhost:15672/)
  
- Credenciais padrão:
  - **Usuário**: guest
  - **Senha**: guest

## 4) Executar:

- Primeiro, execute o comando do servidor:
  ```bash
  python3 rpc_server.py
  ```

- Depois, execute o comando do cliente:
  ```bash
  python3 rpc_client.py
  ```