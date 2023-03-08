# Machine Learning mit Decision Trees
Ein Decision Tree ist ein Machine Learning Algorithmus, der eine Vorhersage (Regression/Klassifikation) anhand von Ja/Nein Entscheidungen in einem Entscheidungsbaum trifft. Es gibt eine große Klasse an effektiven Algorithmen, die auf Entscheidungsbäumen basieren.

## Warum sind tree-based Algorithmen wichtig? 
- sehr effektive Algorithmen bei *tabularen* Daten (SOTA Algorithmen haben teilweise eine höhere Accuracy als neuronale Netze)
- gut interpretierbar
- eignen sich für verschieden Daten, auch mit komplexen, nichtlinearen Zusammenhängen
- relativ robust gegenüber Overfitting und Ausreißern
- schnell zu trainieren, verbrauchen vergleichsweise wenige Daten

## Wofür sind tree-based Algorithmen nicht geeignet?
- unstrukturierte Daten (Bilder, Text, Audio)

## Wie funktioniert ein Entscheidungsbaum?
Einführung: Struktur
### splitting
- Einschränkung auf Regression: Residuenquadratsumme minimieren
### pruning
- Warum? Um Overfitting zu vermeiden und Trainingszeit zu verkürzen
- Hyperparameter: max_depth
- Kreuzvalidierung, um $\alpha$ zu bestimmen

### ensemble methods
- Warum? Ein einzelner Entscheidungsbaum ist leider nicht sonderlich gut als Modell
- Bagging
- random forests (zur Seite)
- boosting (nach unten)
### interpretieren
- scikit-learn: feature_importances_
- SHAP
- permutation importance
## Wichtige Algorithmen, die auf Entscheidungsbäumen basieren 
- random forest
- XGBoost
- Light-GBM

## Anwendung
- scikit-learn
