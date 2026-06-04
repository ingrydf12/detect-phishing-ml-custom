# Detector de emails de phishing com regressão logística
Este projeto implementa um modelo simples de machine learning para identificar e-mails de phishing usando Regressão Logística.

A ideia seria treinar identificar esses emails com objetivo de tentativa de fraude separando de emails legítimos. Também seria suportado a adição de datasets pelo usuário como ``.json`` ou ``.csv`` com base em duas colunas principais: Email Text e Email Type.

## Libs

- sklearn
- joblib
- matplotlib
- seaborn
- scipy
- numpy
- pandas

## Distribuição

![Distribuição da quantidade de emails do tipo SAFE e PHISHING](https://github.com/ingrydf12/detect-phishing-ml-custom/blob/master/docs/distribution.PNG?raw=true)

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