# Exportador SQL e Enviador de E-mail

Este script em Python conecta-se a um banco de dados SQL Server, executa duas consultas SQL (como vendas e estoque), exporta os resultados em arquivos `.csv` e `.txt`, e os envia automaticamente por e-mail.

## 📦 Funcionalidades

- Conexão ao banco de dados SQL Server
- Execução de até duas consultas SQL diferentes
- Exportação dos dados em:
  - Arquivos `.csv` (separador `;`)
  - Arquivos `.txt` (texto plano, delimitado por `;`)
- Envio automático dos arquivos como anexos via e-mail (SMTP)

## 🚀 Requisitos

- Python 3.x
- Pacotes Python:
  - `pandas`
  - `pyodbc`
  - `pytz`
  - `smtplib` (já incluso na biblioteca padrão)
  - `email` (já incluso na biblioteca padrão)

## 🔐 Segurança

A senha do e-mail usada no envio deve ser armazenada em um **arquivo separado chamado `segredo.py`** com a seguinte estrutura:

```python
senha = "sua_senha_de_aplicativo"
