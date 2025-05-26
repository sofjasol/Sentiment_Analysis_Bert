# Sentiment_Analysis_Bert
Посмотрим на то, как модель (dccuchile/bert-base-spanish-wwm-uncased) анализирует тональность.

Можно сказать, что модель справляется с более очевидными предложениями, однако, она совсем, в упор, не понимает сарказма и, вероятно (но не точно), смотрит на ключевые слова.

Примеры работы модели:

1.
```
eval('Hemos perdido el tren por llegar tarde.')
```

```
[{'positive': False, 'probs': array([0.9974733 , 0.00252665], dtype=float32)}]
```

2.
```
eval('El clima hoy es… interesante.')
```

```
[{'positive': True, 'probs': array([0.00137173, 0.99862826], dtype=float32)}]
```
