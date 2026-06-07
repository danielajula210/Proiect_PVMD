# Proiect_PVMD - Clasificarea boabelor uscate de fasole folosind Spark ML

Scopul proiectului este analizarea tipurilor de boabe uscate de fasole din **Dry Bean Dataset**, folosind Apache Spark și biblioteca Spark ML.
S-a creat o analiză locală, utilizând Visual Studio Code, unde a fost creat un Jupyter Notebook, dar și una pe cloud, 
utilizând Databrick, unde s-a creat un Python Notebook, ambele utilizând aceeași manieră și același set de date.

În proiect sunt utilizați trei algoritmi de clasificare:
- Decision Tree
- Random Forest
- Logistic Regression

Datasetul folosit este **Dry Bean Dataset**, disponibil aici:  
https://archive.ics.uci.edu/dataset/602/dry+bean+dataset


## Pași de rulare locală

1. Se clonează repository-ul.
2. Se verifică faptul că fișierul `Dry_Bean_Dataset.csv` se află în același folder cu notebook-ul.
3. Se deschide fișierul `project.ipynb` în VS Code sau Jupyter Notebook.
4. Se selectează un kernel Python.
5. Se rulează celulele notebook-ului în ordine, de sus în jos.
6. La final sunt afișate rezultatele pentru cei trei algoritmi: Accuracy, F1-score și timpul de antrenare.

## Rulare în cloud

Pentru rularea în cloud:
-> dacă utilizatorul face parte din workspace: 
    - proiectul poate fi executat în Databricks. Datasetul se încarcă în Databricks ca tabel, 
      apoi notebook-ul se rulează folosind sesiunea Spark oferită de platformă.
-> dacă utilizatorul nu face parte din workspace:
    - proiectul nu poate fi executat, dar rezultatele pot fi vizualizate accesând fișierul html
      prezent in repository
