# RL Store - Catalogo Online 

## Requisitos do Sistema
- PHP 8.0+
- MariaDB 10.4+
- Servidor Web (Apache/Nginx)
- Navegador Web

## Passos de Instalação

### 1. Configuração da Base de Dados
1. Criar uma nova base de dados MySQL/MariaDB com o nome `pap`
2. Importar o esquema da base de dados a partir do ficheiro `base de dados.txt`
   - Usar phpMyAdmin ou linha de comandos MySQL
   - Este ficheiro contém a estrutura inicial da base de dados e dados de exemplo

### 2. Configuração da Ligação à Base de Dados
- Editar `php/db_connect.php` com as suas credenciais:
```php
<?php
$host = 'localhost';
$username = 'admin';
$password = 'adminpassword';
$database = 'pap';
$conn = new mysqli($host, $username, $password, $database);
```

### 3. Configuração do Servidor Web
- Colocar todos os ficheiros do projeto na raiz do documento do servidor web
- Garantir que o PHP e as extensões necessárias estão ativadas

### 4. Credenciais de Início de Sessão Predefinidas
- Utilizador: `admin`
- Palavra-passe: `adminpassword`

### 5. Funcionalidades
- Autenticação de utilizador
- Navegação de produtos
- Filtragem de produtos
- Gestão de produtos para administrador

### Resolução de Problemas
- Verificar registos de erros do PHP
- Confirmar definições de ligação à base de dados
- Garantir que todas as dependências estão instaladas

### Nota de Segurança
- Alterar credenciais de administrador predefinidas imediatamente
- Implementar medidas de segurança adicionais para produção
