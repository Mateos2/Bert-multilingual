# Bert-multilingual

Este código contiene una clase que carga un modelo BERT multilingüe preentrenado que clasifica si un texto contiene una relación económica válida.

# Requisitos

* Python 3.10+
* Modelo preentrenado: bert_relation_model.pt
* PyTorch
* Transformers

Instalación de bibliotecas:

```python
pip install -r requirements.txt
```

# Uso

Se inicializa el clasificador BERT
```python
clf = RelationClassifier("bert_relation_model.pt")
clf.load_model()
```

Se agrega el texto que se desea predecir
```python
print(clf.predict("Texto a predecir")) # True o False
```
