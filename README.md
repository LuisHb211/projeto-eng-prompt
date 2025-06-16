# Projeto Django - Página de Introdução com Prompt de IA

Este é um projeto Django simples que exibe uma página com texto introdutório e uma área destinada a um prompt de Inteligência Artificial.

---

## Passos para rodar o projeto localmente

1.  **Clone o repositório:**
    ```bash
    git clone [https://github.com/LuisHb211/projeto-eng-prompt.git](https://github.com/LuisHb211/projeto-eng-prompt.git)
    cd seu-repositorio
    ```

2.  **Crie e ative o ambiente virtual:**

    * **Linux / macOS:**
        ```bash
        python3 -m venv venv
        source venv/bin/activate
        ```

    * **Windows:**
        ```bash
        python -m venv venv
        venv\Scripts\activate
        ```

3.  **Instale as dependências:**
    ```bash
    pip install -r requirements.txt
    ```

4.  **Configure as variáveis de ambiente:**
    * Renomeie o arquivo `.env-example` para `.env`:
        * **Linux/macOS:**
            ```bash
            mv .env-example .env
            ```
        * **Windows:**
            ```bash
            ren .env-example .env
            ```
    * Edite o valor de `SECRET_KEY` no arquivo `.env`:
        ```
        SECRET_KEY=sua-chave-secreta-aqui
        ```
    * **Dica:** você pode gerar uma chave com este comando Python:
        ```python
        from django.core.management.utils import get_random_secret_key
        get_random_secret_key()
        ```

5.  **Rode o servidor de desenvolvimento:**
    ```bash
    python manage.py runserver
    ```
    Acesse no navegador: `http://127.0.0.1:8000`

---