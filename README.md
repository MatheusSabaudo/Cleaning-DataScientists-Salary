# 📊 Data Science Salaries Analysis

## 📋 Descrizione del Progetto

Analisi di un dataset di **3.755 stipendi** nel campo della Data Science, coprendo gli anni **2020-2023**.
L'obiettivo è rispondere a 6 domande chiave sul mercato del lavoro dei dati, con particolare attenzione all'impatto della pandemia COVID-19.

## 🎯 Domande di Ricerca

1. **Esiste una correlazione tra livello di esperienza e stipendio?**
2. **Ci sono differenze salariali tra aziende di diverse dimensioni?**
3. **Come si distribuiscono geograficamente i professionisti dei dati?**
4. **Qual è stata la crescita dei professionisti dei dati negli ultimi 4 anni?**
5. **C'è una correlazione tra l'inizio della pandemia e l'aumento dei professionisti?**
6. **Quali sono i professionisti più pagati nel settore?**

## 🛠️ Tecnologie Utilizzate

* **Python 3.13**
* **Pandas** - Manipolazione e analisi dati
* **NumPy** - Calcoli numerici
* **Matplotlib** - Visualizzazioni base
* **Seaborn** - Visualizzazioni statistiche avanzate
* **SciPy** - Test statistici (ANOVA, t-test)

## 📁 Struttura del Progetto

```
Data-Cleaning.ipynb          # Notebook principale con analisi completa
data/
└── ds_salaries.csv          # Dataset originale
README.md                    # Documentazione del progetto
```

## 🔍 Analisi Eseguita

### 1. Data Cleaning & Preprocessing

* Conversione dei codici dei livelli di esperienza (SE → Senior-Level, MI → Mid-Level, EN → Entry-Level, EX → Executive-Level)
* Conversione dei tipi di impiego (FT → Full-Time, CT → Contract, FL → Freelance, PT → Part-Time)
* Conversione delle dimensioni aziendali (L → Large, M → Medium, S → Small)
* Impostazione dell'ordine categorico per le variabili ordinali

### 2. Analisi Statistiche

* **ANOVA** per confrontare le medie tra gruppi
* **T-test** per confronti a coppie
* **Statistiche descrittive** (media, mediana, deviazione standard)
* **Calcolo CAGR** (Compound Annual Growth Rate)

### 3. Visualizzazioni

* Boxplot per distribuzioni salariali
* Bar chart per confronti categorici
* Time series per trend temporali
* Heatmap per correlazioni geografiche

## 📊 Risultati Principali

### 📈 Crescita del Settore

* **2020**: 76 posizioni
* **2023**: 1.785 posizioni
* **Crescita totale**: +2.249%
* **CAGR**: +186.4%

### 💰 Stipendi per Esperienza

| Livello         | Stipendio Medio | Premium vs Entry-Level |
| --------------- | --------------- | ---------------------- |
| Entry-Level     | $78.546         | -                      |
| Mid-Level       | $104.526        | +33%                   |
| Senior-Level    | $153.051        | +95%                   |
| Executive-Level | $194.931        | +148%                  |

### 🏢 Stipendi per Dimensione Aziendale

| Dimensione | Stipendio Medio | Premium vs Small |
| ---------- | --------------- | ---------------- |
| Small      | $78.227         | -                |
| Medium     | $143.131        | +83%             |
| Large      | $118.301        | +51%             |

### 🌍 Distribuzione Geografica

* **USA**: 81% delle posizioni (3.040)
* **UK**: 4.6% (172)
* **Canada**: 2.3% (87)
* **Spagna**: 2.1% (77)

### 🦠 Impatto Pandemia

* **Crescita post-pandemia**: +4.741%
* **Stipendio pre-pandemia**: $92.303
* **Stipendio pandemia**: $138.506
* **Incremento salariale**: +50.1%

### 🏆 Ruoli Più Pagati

| Ruolo                              | Stipendio Medio |
| ---------------------------------- | --------------- |
| Principal Data Scientist           | $198.171        |
| Director of Data Science           | $195.141        |
| Machine Learning Software Engineer | $192.420        |
| Data Science Manager               | $191.279        |
| Applied Scientist                  | $190.264        |

## 📈 Test Statistici

### ANOVA - Esperienza vs Stipendio

* **F-statistic**: 245.67
* **p-value**: < 0.001
* **Conclusione**: Correlazione statisticamente significativa

### ANOVA - Dimensione Azienda vs Stipendio

* **F-statistic**: 89.23
* **p-value**: < 0.001
* **Conclusione**: Differenze significative tra dimensioni

## 💡 Key Takeaways

1. **L'esperienza paga**: I Senior-Level guadagnano il doppio degli Entry-Level
2. **Le medie aziende pagano meglio**: Contrariamente all'aspettativa, le aziende medie pagano più delle grandi
3. **USA domina il mercato**: L'81% delle posizioni sono negli Stati Uniti
4. **Boom pandemico**: Crescita esplosiva (+623% nel 2022) post-pandemia
5. **Specializzazione richiesta**: Ruoli di machine learning e data science leadership sono i più pagati

## 🚀 Come Eseguire

```bash
# Clona il repository
git clone https://github.com/MatheusSabaudo/Cleaning-DataScientists-Salary.git

# Installa le dipendenze
pip install pandas numpy matplotlib seaborn scipy

# Apri il notebook
jupyter notebook Data-Cleaning.ipynb
```

## 📝 Note

* Il dataset include solo posizioni con stipendio in USD convertito
* I test statistici sono stati eseguiti con α = 0.05
* Per affidabilità statistica, sono state considerate solo posizioni con ≥ 5 occorrenze per l'analisi dei ruoli

## 📚 Fonti

* Dataset: [Data Science Salaries su Kaggle](https://www.kaggle.com/datasets/ruchi798/data-science-job-salaries)
* Anni coperti: 2020-2023

## ✨ Autore

Matheus Sabaudo Rodrigues - Analisi dati completa con focus su trend di mercato e impatto pandemia
