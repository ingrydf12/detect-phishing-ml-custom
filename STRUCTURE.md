# Project Structure

detect-phishing-ml-custom/
│
├── data/
│   ├── raw/            # dados originais
│   ├── processed/      # dados tratados
│   └── external/       # dados customizados
│
├── notebooks/          # exploração (EDA, testes rápidos)
│
├── src/
│   ├── data/           # scripts de coleta e preprocessamento
│   ├── features/       # engenharia de features
│   ├── models/         # treino e avaliação
│   ├── utils/          # funções auxiliares
│   └── config/         # configs do projeto
│
├── models/             # modelos treinados (.pkl, .pt, etc)
│
├── reports/
│   ├── figures/        # gráficos e imagens
│   └── metrics/        # resultados e métricas
│
├── tests/              # testes (não utilizado ainda)
│
├── .env                # variáveis de ambiente
├── .gitignore
├── requirements.txt
├── README.md
└── main.py             # entry point


# Run

```bash
python -m venv venv
source venv/bin/activate
pip install -r requirements.txt

python main.py