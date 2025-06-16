Projeto Django - Página de Introdução com Prompt de IA

Este é um projeto Django simples que exibe uma página com texto introdutório e uma área destinada a um prompt de Inteligência Artificial.

----------------------------------------
Passos para rodar o projeto localmente
----------------------------------------

1. Clone o repositório:

    git clone https://github.com/seu-usuario/seu-repositorio.git
    cd seu-repositorio

2. Crie e ative o ambiente virtual:

    # Linux / macOS
    python -m venv venv
    source venv/bin/activate

    # Windows
    python -m venv venv
    venv\Scripts\activate

3. Instale as dependências:

    pip install -r requirements.txt

4. Configure as variáveis de ambiente:

    - Renomeie o arquivo .env-example para .env

        # Linux/macOS
        mv .env-example .env

        # Windows
        ren .env-example .env

    - Edite o valor de SECRET_KEY no arquivo .env:

        SECRET_KEY=sua-chave-secreta-aqui

    - Dica: você pode gerar uma chave com este comando Python:

        from django.core.management.utils import get_random_secret_key
        get_random_secret_key()

5. Rode o servidor de desenvolvimento:

    python manage.py runserver

    Acesse no navegador:
    http://127.0.0.1:8000


----------------------------------------
Estrutura de Diretórios (resumida)
----------------------------------------

├── manage.py
├── .env-example
├── requirements.txt
├── static/
│   └── css/
│       └── intro.css
├── templates/
│   └── intro.html
├── app/
│   ├── views.py
│   └── urls.py
└── ...


Observações:

- O arquivo HTML principal está em templates/intro.html
- O CSS está em static/css/intro.css
- O projeto utiliza variáveis de ambiente para manter a SECRET_KEY segura

Feito com 💻 por [Seu Nome]
