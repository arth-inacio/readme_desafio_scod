# 🕵️‍♂️ SCOD Scraping Challenge

Bem-vindo(a) ao **Desafio de Estágio - SCOD Solutions**!  
Este teste tem como objetivo avaliar sua capacidade de **coletar dados (web scraping)**, organizar informações e automatizar pequenas tarefas com boas práticas de código.

---

## 🚀 Desafio

Acesse a seguinte página de teste:
🔗 **[https://arth-inacio.github.io/scod_scraping_challenge/](https://arth-inacio.github.io/scod_scraping_challenge/)**

### Sua missão:
1. Fazer o **scraping** da tabela de débitos exibida na página.  
2. Fazer o **download dos boletos (PDFs)** disponíveis em cada linha.  
3. **Salvar os dados extraídos** (descrição, exercício, parcela, vencimento, valor, status e link do boleto) em um arquivo JSON.  
4. Utilizar uma das seguintes abordagens para a coleta:
   - `requests` ou `httpx`
   - `async-httpx`
   - `selenium`
   - `playwright` ou `async-playwright`

---

## 🧩 Requisitos

- O código deve estar **bem estruturado e legível**.
- Pode ser desenvolvido em **Python 3.9+**.
- Utilize **orientação a objetos (OOP)** se possível (será considerado um diferencial).
- Organize seu projeto em pastas claras (ex: `src/`, `data/`, `boletos/`).
- Inclua um **arquivo `requirements.txt`** com as dependências necessárias.
- O script principal pode ser chamado, por exemplo, `main.py`.

---

## 📦 Saída esperada

Ao final da execução, o projeto deve gerar:

- Um arquivo `dados.json` contendo todos os registros da tabela.
- Uma pasta `boletos/` com os arquivos PDF baixados.

Exemplo do formato do `dados.json`:

```json
[
  {
    "descricao": "IPTU - Taxa Municipal",
    "exercicio": 2024,
    "parcela": "1/3",
    "vencimento": "2024-04-30",
    "valor": 1234.56,
    "status": "Vencido",
    "boleto_url": "boletos/18164829.pdf"
  }
]
