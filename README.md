# 🗨️ Chat Terminal Simples em Python

Este é um projeto simples em Python que simula um chat no terminal. Ele permite que o usuário insira mensagens em tempo real, que são armazenadas e exibidas em uma interface de linha de comando.

# 🚀 Funcionalidades

- Entrada de nome do usuário

- Inserção de múltiplas mensagens

- Exibição em tempo real das mensagens anteriores

- Encerramento do chat ao digitar fim

# 📦 Requisitos

- Python 3.x

# ▶️ Como usar

1. Clone o repositório ou copie o código para um arquivo .py, por exemplo: main.py

2. Execute o script: python main.py

3. Insira seu nome quando solicitado.

4. Digite suas mensagens uma a uma.

5. Para encerrar, digite: fim

# 🧠 Exemplo de uso
Nome: Thaciane

_________________
mensagem: Olá, tudo bem?

Thaciane - Olá, tudo bem?
_________________
mensagem: Estou testando esse chat.

Thaciane - Olá, tudo bem?

Thaciane - Estou testando esse chat.
_________________
mensagem: fim

# 📁 Código-fonte

    import os 

    mensagens = []

    nome = input("Nome: ")

    while True:

        # limpando terminal
        os.system('cls')

        if len(mensagens) > 0:
        for m in mensagens:
            print(m['nome'], "-", m['texto'])

        print("_________________")

        # obtendo texto
        texto = input("mensagem: ")
        if texto == "fim":
            break

        # adicionando mensagem na lista 
        mensagens.append({
            "nome": nome,
            "texto": texto
        })
