# Coleta e Tratamento de Dados do IPCA (API Banco Central)

Projeto para coleta, verificação e tratamento de dados públicos do IPCA (últimos 20 meses) em formato JSON, via API oficial do Banco Central do Brasil (SGS). Utiliza a biblioteca Pandas para limpeza e conversão de tipos, com exportação final nos formatos CSV e Parquet.

## Tecnologias Utilizadas

- **Python:** Linguagem de programação principal utilizada em toda a codificação do projeto.
- **Requests:** Biblioteca utilizada para realizar requisições HTTP (`requests.get`) à API do Banco Central.
- **Pandas:** Biblioteca utilizada para estruturar os dados em tabela (`DataFrame`), fazer o diagnóstico inicial, realizar o tratamento e exportar os arquivos.
- **PyArrow:** Motor instalado para permitir que o Pandas salve e leia os dados no formato profissional `.parquet`.
- **Jupyter Notebook (VS Code):** Ambiente interativo utilizado dentro do editor VS Code para combinar células de código executável e documentação em Markdown no mesmo arquivo (`.ipynb`).

## Estrutura de Pastas

```text
modulo_18_bcb/
├── data/
│   ├── raw/
│   │   └── bcb_tabela.csv
│   └── processed/
│       ├── dados_tratados.csv
│       └── dados_tratados.parquet
├── notebooks/
│   └── pratique_ibge_bcb.ipynb
└── README.md
```

## Como Executar o Projeto

1. Instale as bibliotecas necessárias executando o comando abaixo no terminal:

```bash
pip install requests pandas pyarrow
```
2. Abra o arquivo `notebooks/pratique_ibge_bcb.ipynb` no VS Code ou Jupyter Notebook.

3. Execute as células em ordem para gerar os arquivos nas pastas `data/raw` e `data/processed`.


## Fonte dos Dados

- **Banco Central do Brasil (SGS):** [Portal de Dados Abertos](https://dadosabertos.bcb.gov.br/) — Série 433 (IPCA mensal).

## Autor

Desenvolvido por **João Paulo Ferreira** — [GitHub](https://github.com/paulloxuesheng) | [LinkedIn](https://www.linkedin.com/in/joaopaulo-ferreira-tech)