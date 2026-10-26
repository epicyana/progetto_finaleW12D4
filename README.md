# praticaW12D4
# ToysGroup in Python: dal dato grezzo al modello

Esercitazione finale del Modulo 4 (Python for Data Science, Epicode Institute of Technology).

## Lo scenario
ToysGroup distribuisce giocattoli attraverso una rete di rivenditori in diversi paesi europei. In questo progetto leggo, pulisco, analizzo e modello i dati di vendita, per capire come va il fatturato nel tempo, quali categorie e aree rendono di più e quali rivenditori rischiano di smettere di ordinare.

## I dati
| File | Contenuto |
|---|---|
| `products.csv` | 12 prodotti con categoria e prezzo di listino |
| `regions.xlsx` | 9 paesi con la loro area di vendita (Sud, Centro, Nord Europa) |
| `sales.json` | 2000 vendite dal 2023 al 2025, con alcuni valori mancanti in quantità e importo |
| `resellers.csv` | 300 rivenditori con ordini, giorni dall'ultimo ordine, sconto, reclami e abbandono (churn) |

## I task
1. **Python di base:** liste, dizionari, set, cicli e funzioni, senza i metodi di analisi di Pandas.
2. **Lettura e ispezione:** DataFrame, `.describe()`, array NumPy, `.loc[]` e `.iloc[]`.
3. **Pulizia e analisi:** valori mancanti, filtri e ordinamenti (3a), unione delle tabelle e aggregazioni (3b), serie temporali (3c).
4. **Visualizzazione:** grafico a linee (Matplotlib), boxplot e heatmap (Seaborn), barre interattive (Plotly).
5. **Regressione lineare:** previsione del fatturato mensile con un modello semplice e uno multiplo.
6. **Machine learning:** previsione dell'abbandono dei rivenditori con la regressione logistica (6a) e divisione dei rivenditori in gruppi con K-Means (6b).
7. **Debugging e versioning:** correzione di quattro frammenti di codice sbagliati e pubblicazione del progetto su GitHub.

## Alcuni risultati
- Dopo la pulizia le vendite sono 1900, e il fatturato totale è di circa 560.000 €.
- Outdoor è la categoria che fattura di più (circa 332.000 €), e il Centro Europa è l'area più forte.
- Il fatturato cresce del 21% nel 2025 rispetto al 2024, con il picco a maggio 2025 (circa 29.400 €).
- Il modello per prevedere l'abbandono individua circa 7 rivenditori su 10 che smettono di ordinare, usando la soglia 0,3.
- Il segmento "In allontanamento" (137 rivenditori) raccoglie circa tre abbandoni su quattro.

## Come eseguire il progetto
1. Scarica o clona il repository, tenendo il notebook e i quattro file di dati nella stessa cartella.
2. Installa le librerie necessarie:
   ```
   pip install pandas numpy matplotlib seaborn plotly scikit-learn openpyxl jupyter
   ```
3. Apri il notebook con Jupyter:
   ```
   jupyter notebook Progetto_Finale.ipynb
   ```
4. Scegli **Kernel → Restart Kernel and Run All Cells**: il notebook va eseguito dall'inizio, nell'ordine delle celle.

## Contenuto del repository
- `Progetto_Finale.ipynb`: il notebook con tutti i task.
- `products.csv`, `regions.xlsx`, `sales.json`, `resellers.csv`: i dati di partenza.

## Nota sull'uso dell'AI
Nel Task 7 ho usato un assistente AI per individuare la causa degli errori nei quattro frammenti, come richiesto dalla consegna. Nel notebook sono riportati, per ciascun caso, il codice originale, l'errore, la causa, la correzione e il prompt usato.
