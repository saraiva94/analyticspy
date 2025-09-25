# AnalyticsPy

Projeto de análise exploratória e modelagem inicial focado em **cancelamentos** (churn), com notebooks em Python e conjunto(s) de dados CSV. A proposta é entregar um pipeline simples e reproduzível para inspeção, limpeza, visualização e primeiros modelos/insights.

## 🎯 Objetivos
- Entender variáveis associadas a **cancelamentos**.
- Construir **EDA** clara (valores ausentes, distribuição, correlações).
- Criar **baseline** de modelos simples (opcional) e métricas rápidas.
- Documentar um caminho de reprodução local.

## 🗂 Estrutura (esperada)
```
.
├─ cancelamentos.csv                 # dataset principal
├─ cancelamentos_sample.csv          # amostra para testes rápidos
├─ inicial.ipynb                     # EDA e preparação de dados
├─ gabarito.ipynb                    # referência/solução-base (baseline/etapas finais)
└─ README.md
```

> Se a sua estrutura diferir, ajuste este bloco conforme necessário.

## 🔧 Requisitos
- Python 3.10+
- Bibliotecas (sugestão):
  - pandas
  - numpy
  - matplotlib
  - plotly
  - seaborn
  - scikit-learn
  - jupyter

## 🚀 Instalação rápida
```bash
# 1) Crie e ative um ambiente virtual (opcional, mas recomendado)
python -m venv .venv
# Windows
.venv\Scripts\activate
# macOS/Linux
source .venv/bin/activate

# 2) Instale as dependências
pip install -U pip
pip install pandas numpy matplotlib plotly seaborn scikit-learn jupyter
```

> Se você usar `requirements.txt`, substitua pelo:
```bash
pip install -r requirements.txt
```

## ▶️ Como rodar
```bash
# Abrir o Jupyter
jupyter notebook
```
- Abra **`inicial.ipynb`** para executar a EDA passo a passo.
- Em seguida, rode **`gabarito.ipynb`** para baseline/modelos/métricas (quando aplicável).

## 🧪 Dados
- **`cancelamentos.csv`**: base completa (campos e dicionário variam conforme a origem).
- **`cancelamentos_sample.csv`**: subconjunto menor para iteração rápida.
- Recomendações:
  - Verificar encoding (`utf-8` vs `latin-1`).
  - Conferir separador (`;` vs `,`).
  - Padronizar tipos (datas, numéricos, categóricos).

## 🧱 Boas práticas
- Manter **seed** fixa para reprodutibilidade.
- Salvar artefatos (ex.: CSV tratados) em `data/processed/` (se criar a pasta).
- Versionar notebooks limpos (evite outputs gigantes).

## 🗺 Roadmap
- [ ] Dicionário de dados (coluna a coluna).
- [ ] Pipeline de limpeza (funções reutilizáveis).
- [ ] Notebooks separados: `01-eda.ipynb`, `02-modelo-baseline.ipynb`.
- [ ] Export de relatórios (HTML/PDF) com resultados.
- [ ] `requirements.txt` / `pyproject.toml`.

## 🤝 Contribuição
1. Crie uma branch: `git checkout -b feat/minha-feature`
2. Commits descritivos.
3. Abra um PR explicando o que mudou e por quê.

