# Detector de emails de phishing
Este projeto implementa um modelo simples de machine learning para identificar e-mails de phishing usando Naive Bayes Multinomial simples.

A ideia seria treinar identificar esses emails com objetivo de tentativa de fraude separando de emails legítimos. Também seria suportado a adição de datasets pelo usuário como ``.json`` ou ``.csv`` com base em duas colunas principais: Email Text e Email Type.

## Dataset utilizado

Deve ser baixado e importado para a pasta de datasets para rodar o projeto.

https://huggingface.co/datasets/RonakAJ/phising_email


## Estrutura do projeto

```
detect-phishing-ml-custom/
│
├── datasets/
├── models/ # modelos treinados (.pkl, .pt, etc)
├── src/
│   ├── Phishing_Project.ipynb - Notebook
├── .gitignore
├── requirements.txt
├── README.md
```

# Rodar o projeto

```bash
python -m venv venv
source venv/bin/activate
pip install -r requirements.txt

python main.py