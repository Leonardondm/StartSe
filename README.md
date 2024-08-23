# StartSe

StartSe é uma plataforma web desenvolvida para facilitar a conexão entre startups e investidores. Empresas podem se cadastrar para vender suas ações, enquanto investidores podem explorar o catálogo de empresas disponíveis para realizar investimentos.

## Funcionalidades

- **Cadastro de Startups**: Empresas podem criar perfis, fornecer detalhes sobre suas startups, e listar ações disponíveis para venda.
- **Sistema de Investimentos**: Investidores podem buscar startups, visualizar informações detalhadas das empresas, e decidir sobre seus investimentos.
- **Busca de Empresas**: Investidores podem usar filtros para encontrar startups de acordo com interesses específicos, como área de atuação e valor de investimento.
- **Gerenciamento de Perfis**: Startups podem atualizar suas informações a qualquer momento para manter seu perfil atrativo aos investidores.

## Tecnologias Utilizadas

- **Linguagem de Programação**: Python 3.9
- **Framework Backend**: Django (Framework Web em Python)
- **Banco de Dados**: SQLite (padrão Django)
- **Frontend**: HTML5, CSS3, JavaScript
- **Template Engine**: Django Templating Language

### Descrição dos Principais Diretórios e Arquivos:

- **core/**: Contém os arquivos de configuração e as rotas principais da aplicação.
  - `settings.py`: Configurações do projeto Django (banco de dados, apps instalados, middleware, etc).
  - `urls.py`: Arquivo responsável por mapear as URLs para as views correspondentes.

- **empresarios/**: App dedicado ao cadastro e gerenciamento de startups.
  - `views.py`: Lida com as requisições relacionadas ao cadastro e gerenciamento de empresas.
  - `models.py`: Contém os modelos de dados relacionados às startups, como nome da empresa, descrição, ações disponíveis, etc.
  - `templates/empresarios/`: Armazena os templates HTML relacionados às páginas de empresas.

- **investidores/**: App dedicado aos investidores que buscam startups para investir.
  - `views.py`: Lida com as requisições relacionadas à busca e visualização de startups.
  - `models.py`: Contém os modelos de dados relacionados aos investidores.
  - `templates/investidores/`: Armazena os templates HTML relacionados às páginas de investidores.

- **db.sqlite3**: Banco de dados SQLite, contendo todas as informações da aplicação (startups, investidores, etc).

- **manage.py**: Script de gerenciamento do Django, utilizado para executar comandos como iniciar o servidor, aplicar migrações, entre outros.

- **requirements.txt**: Arquivo com as dependências do projeto. Todas as bibliotecas necessárias podem ser instaladas usando o comando `pip install -r requirements.txt`.

## Instalação e Configuração

Siga os passos abaixo para configurar e rodar o projeto localmente:

1. **Clone o repositório**:
  ```bash
  git clone https://github.com/Leonardondm/StartSe.git
  ```
2. **Navegue até o diretório do projeto**:
  ```bash
  cd StartSe-main
  ```
3. **Crie e ative um ambiente virtual**:
  ```bash
  python -m venv venv
  source venv/bin/activate  # No Windows: venv\Scripts\activate
  ```
4. **Instale as dependências do projeto**:
  ```bash
  git clone https://github.com/Leonardondm/StartSe.git
  ```
5. **Realize as migrações do banco de dados**:
  ```bash
  python manage.py migrate
  ```
6. **Inicie o servidor de desenvolvimento**:
  ```bash
  python manage.py runserver
  ```
7. **Acesse a aplicação: Abra o navegador e vá para http://localhost:8000 para visualizar a aplicação.**
