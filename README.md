# Chat Cliente/Servidor

Este é um aplicativo de chat seguro desenvolvido usando `customtkinter` para a interface gráfica, `socket` para comunicação em rede e `hashlib` para armazenamento seguro de senhas em Python. Ele possui autenticação de usuário, um cliente de chat em tempo real e um servidor com filtro de palavrões.

## Funcionalidades

* **Autenticação de Usuário**: Os usuários podem criar novas contas e fazer login com suas credenciais. As senhas são armazenadas de forma segura usando hash SHA-256.
* **Chat em Tempo Real**: Os usuários podem trocar mensagens em um ambiente de chat em tempo real.
* **Filtro de Palavrões**: O servidor censura palavras profanas predefinidas nas mensagens antes de transmiti-las para outros usuários.
* **Suporte a Múltiplos Clientes**: O servidor pode lidar com várias conexões de clientes simultâneas usando threading.
* **Interface Gráfica do Usuário (GUI)**: Uma interface amigável é fornecida tanto para o login quanto para o cliente de chat, construída com `customtkinter`.

## Tecnologias Utilizadas

* **Python 3**: A linguagem de programação principal.
* **`customtkinter`**: Para criar interfaces gráficas de usuário modernas e personalizáveis.
* **`socket`**: Para estabelecer conexões de rede entre o cliente e o servidor.
* **`threading`**: Para lidar com múltiplas conexões de clientes simultaneamente no lado do servidor.
* **`hashlib`**: Para hash seguro de senhas (SHA-256).
* **`PIL (Pillow)`**: Usado para manipulação de imagens na GUI (por exemplo, carregar e redimensionar imagens).
* **`json`**: Para armazenar dados do usuário em um arquivo JSON.
* **`re`**: Para operações de expressão regular, especificamente usado no filtro de palavrões.

## Primeiros Passos

### Pré-requisitos

* Python 3.x instalado em seu sistema.
* Bibliotecas Python necessárias. Você pode instalá-las usando pip:

    ```bash
    pip install customtkinter Pillow
    ```

### Instalação

1.  **Clone o repositório:**
    ```bash
    git clone <url_do_repositorio>
    cd <nome_do_repositorio>
    ```
2.  **Certifique-se de que todos os arquivos Python fornecidos estão no mesmo diretório:**
    * `login.py`
    * `servidor.py`
    * `cliente_gui.py`
    * `usuarios_db.py`
3.  **Coloque os arquivos de imagem necessários no mesmo diretório:**
    * `Rio1.png`
    * `Logo.png`
    * `user2.png`
    * `senha3.png`

### Executando o Aplicativo

1.  **Iniciar o Servidor:**
    Abra um terminal ou prompt de comando e execute o script do servidor:

    ```bash
    python servidor.py
    ```
    Você deve ver uma mensagem indicando que o servidor foi iniciado e está aguardando conexões.
2.  **Iniciar o Cliente (Interface de Login):**
    Abra outro terminal ou prompt de comando e execute o script de login:

    ```bash
    python login.py
    ```
    Isso abrirá a janela de login.
3.  **Criar uma Conta ou Fazer Login:**
    * **Criar Conta**: Clique em "Criar conta" para abrir uma nova janela onde você pode registrar um novo nome de usuário e senha.
    * **Fazer Login**: Se você já tiver uma conta, digite seu nome de usuário e senha nos campos respectivos e clique em "Login".
4.  **Conversando:**
    Uma vez logado, a janela do cliente de chat aparecerá. Você pode digitar suas mensagens no campo de entrada e pressionar Enter ou clicar no botão "Enviar" para enviá-las.

## Créditos

Desenvolvido por [Attashiie](https://github.com/Attashiie), [Carlosh007](https://github.com/Carlosh007)
