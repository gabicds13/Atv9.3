# Exercício 9.3 - Flask e Nuvem

Aplicação Hello World em Flask para deploy no Azure App Service via GitHub Actions.

## Rodar localmente

```bash
python -m pip install -r requirements.txt
python app.py
```

Acesse http://127.0.0.1:5000/ no navegador.

## Azure App Service

- Sistema operacional: Linux
- Runtime: Python (mesma versão usada no workflow do GitHub Actions)
- Plano: Free F1 se disponível e desejado
- Arquivo inicial: `app.py` na raiz do repositório
- Se necessário, Startup Command: `gunicorn --bind=0.0.0.0 --timeout 600 app:app`
- Deployment Center: GitHub / GitHub Actions / branch main

## Entrega

- Link do repositório GitHub
- Link da aplicação online no Azure
