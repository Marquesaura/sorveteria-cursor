# Sistema de Controle de Estoque e Vendas

Sistema web para controle de estoque, cadastro de produtos, funcionários, clientes e vendas.

## Funcionalidades

### Cadastro de Produtos
- Registro de produtos com ID, quantidade, tipo, data de chegada, data de vencimento, fornecedor e preço
- Validação de campos obrigatórios
- Formatação automática de valores monetários
- Controle de estoque

### Cadastro de Funcionários
- Registro de funcionários com ID, nome completo, CPF, RG e setor
- Validação de CPF
- Validação de idade mínima (18 anos)
- Verificação de CPF duplicado

### Cadastro de Clientes
- Registro de clientes com ID, nome, CPF, telefone, endereço e email
- Validação de CPF
- Validação de email
- Máscara para CPF e telefone
- Endereço completo com CEP, rua, número, bairro, cidade e estado

### Registro de Vendas
- Vinculação de clientes, produtos e funcionários
- Seleção múltipla de produtos
- Cálculo automático de subtotal e total
- Controle de estoque automático
- Diferentes formas de pagamento
- Visualização detalhada das vendas

## Tecnologias Utilizadas

- HTML5
- CSS3
- JavaScript
- Bootstrap 4
- p5.js
- LocalStorage para persistência de dados

## Recursos

- Layout responsivo
- Validações em tempo real
- Máscaras de entrada
- Mensagens de feedback
- Interface intuitiva
- Persistência de dados no navegador

## Como Usar

1. Clone este repositório
2. Abra o arquivo `index.html` em um navegador web moderno
3. Comece cadastrando produtos e funcionários
4. Cadastre clientes
5. Registre vendas vinculando clientes, produtos e funcionários

## Estrutura do Projeto

```
/
├── index.html
├── css/
│   └── styles.css
├── js/
│   └── main.js
└── pages/
    ├── produtos.html
    ├── funcionarios.html
    ├── clientes.html
    └── vendas.html
```

## Validações Implementadas

- CPF: Verificação de dígitos verificadores e formato
- Email: Formato válido
- Datas: Validação de datas válidas
- Idade: Mínimo 18 anos para funcionários
- Campos obrigatórios: Verificação antes do envio
- Estoque: Controle de quantidade disponível
- Duplicidade: Verificação de CPF duplicado

## Armazenamento

O sistema utiliza o LocalStorage do navegador para persistir os dados. Os dados são salvos nas seguintes chaves:

- `produtos`: Lista de produtos cadastrados
- `funcionarios`: Lista de funcionários
- `clientes`: Lista de clientes
- `vendas`: Registro de vendas

## Melhorias Futuras

- Implementar backend para persistência em banco de dados
- Adicionar sistema de autenticação
- Implementar relatórios e gráficos
- Adicionar busca e filtros nas listagens
- Implementar sistema de backup
- Adicionar foto para produtos
- Implementar impressão de comprovantes
- Adicionar histórico de alterações 