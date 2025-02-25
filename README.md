# Sistema Bancário em Python

Bem-vindo ao **Sistema Bancário em Python**! Este projeto é um exemplo de um sistema bancário simples, desenvolvido em Python, que permite a criação de clientes, contas correntes, e a realização de operações bancárias básicas como depósitos, saques e consultas de extrato.

## Funcionalidades

- **Cadastro de Clientes**: Crie clientes com nome, data de nascimento, CPF e endereço.
- **Criação de Contas**: Associe contas correntes aos clientes cadastrados.
- **Depósitos**: Realize depósitos em contas existentes.
- **Saques**: Efetue saques respeitando limites diários e de valor.
- **Extrato**: Consulte o extrato bancário para visualizar todas as transações realizadas.

## Como Usar

1. **Clonar o Repositório**:
   ```bash
   git clone https://github.com/seu-usuario/sistema-bancario-python.git
   cd sistema-bancario-python
2. **Executar o Projeto**:
   python main.py

   Menu de Opções:

[d] Depositar

[s] Sacar

[e] Extrato

[nc] Nova conta

[lc] Listar contas

[nu] Novo usuário

[q] Sair

Estrutura do Projeto
Cliente: Representa um cliente do banco, com informações pessoais e uma lista de contas associadas.

Conta: Classe base para contas bancárias, com funcionalidades como depósito e saque.

ContaCorrente: Herda de Conta e implementa limites de saque e valor.

Transacao: Classe abstrata que define as operações de transação.

Historico: Mantém um registro de todas as transações realizadas em uma conta.

Exemplo de Uso
python
Copy
# Criar um novo cliente
cliente = PessoaFisica(nome="João Silva", data_nascimento="01-01-1990", cpf="12345678900", endereco="Rua ABC, 123")

# Criar uma nova conta corrente
conta = ContaCorrente.nova_conta(cliente, numero=1)

# Realizar um depósito
conta.depositar(100.0)

# Realizar um saque
conta.sacar(50.0)

# Exibir extrato
conta.historico.transacoes
Contribuição
Contribuições são bem-vindas! Sinta-se à vontade para abrir issues e pull requests para melhorar este projeto.

Licença
Este projeto está licenciado sob a licença MIT - veja o arquivo LICENSE para mais detalhes.

Feito com ❤️ por Malu Freitas
