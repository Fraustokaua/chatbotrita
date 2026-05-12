# 🤖 Bot Paneas

Bem-vindo ao **Bot Paneas**! Este é um assistente virtual inteligente construído com tecnologias robustas como **Python**, **Flask**, **SQLite** e **scikit-learn**. Ele foi desenvolvido especialmente para auxiliar em questões financeiras do dia a dia, fornecendo respostas rápidas e diretas sobre saldos, extratos, transações Pix, cartões de crédito, pagamentos, empréstimos, segurança da conta e até mesmo direcionando para o atendimento humano quando necessário.

---

## 🛠️ Stack Tecnológico

O projeto utiliza um conjunto simples, mas poderoso de tecnologias:
- **Linguagem Principal:** Python
- **Framework Web:** Flask
- **Banco de Dados:** SQLite
- **Machine Learning (IA):** scikit-learn
- **Frontend:** HTML, CSS e JavaScript (Vanilla)

---

## 📁 Estrutura do Projeto

Abaixo você confere a nova organização do projeto em português:

```text
Bot_Paneas/
├── app.py                  # Ponto de entrada do servidor web
├── requirements.txt        # Dependências do projeto
├── LEIAME.md               # Este arquivo
├── .gitignore              # Arquivos ignorados pelo Git
├── dados/                  # Base de conhecimento inicial
│   ├── perguntas.csv
│   └── respostas.json
├── instancia/              # Onde o banco de dados local será salvo
│   └── .gitkeep
├── roteiros/               # Scripts utilitários do projeto
│   └── iniciar_bd.py
├── codigo_fonte/           # O coração do nosso bot (código fonte principal)
│   ├── __init__.py
│   ├── chatbot.py
│   └── banco_dados.py
├── estatico/               # Arquivos estáticos servidos no front
│   ├── estilos/
│   │   └── estilos.css
│   └── scripts/
│       └── chat.js
└── modelos/                # Nossos templates HTML
    └── index.html
```

---

## 🚀 Guia de Inicialização

Siga os passos abaixo para rodar o Bot Paneas na sua máquina local:

### 1. Prepare o Ambiente Virtual
Recomendamos criar um ambiente isolado para não conflitar com outras bibliotecas globais:
```bash
python -m venv venv
venv\Scripts\activate
```

### 2. Instale as Dependências
Com o ambiente ativado, instale os pacotes necessários:
```bash
pip install -r requirements.txt
```

### 3. Inicialize o Banco de Dados
Gere a estrutura inicial e popule os dados a partir dos arquivos locais:
```bash
python roteiros/iniciar_bd.py
```

### 4. Ligue os Motores!
Inicie o servidor localmente:
```bash
python app.py
```

### 5. Acesse o Assistente
Abra o seu navegador favorito e acesse a interface do chat:
`http://127.0.0.1:5000`

---

## 💾 Sobre o Banco de Dados

Toda vez que você rodar o script de inicialização, o banco `chatbot.db` será criado (ou atualizado) dentro da pasta `instancia/`. Ele utiliza as informações contidas em `dados/perguntas.csv` e `dados/respostas.json`.

> ⚠️ **Nota Importante**: O arquivo `.db` gerado está configurado no `.gitignore` para que não seja enviado acidentalmente ao repositório, garantindo que o histórico de conversas dos usuários locais fique privado na sua máquina.

---

## 🗣️ O que posso perguntar?

Fique à vontade para testar as capacidades da inteligência artificial fazendo perguntas como:
- *"Oi, tudo bem?"*
- *"Como vejo meu saldo?"*
- *"Quero fazer um pix"*
- *"Perdi meu cartao, e agora?"*
- *"Qual é o meu limite?"*
- *"Preciso bloquear minha conta"*
- *"Quero ver meu extrato"*
- *"Esqueci minha senha de acesso"*
- *"Quero falar com um atendente humano"*
