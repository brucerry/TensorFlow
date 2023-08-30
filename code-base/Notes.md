#### activation
- sigmoid - binary classification
- softmax - multiclass classification

#### loss
- BinaryCrossentropy - binary classification
- CategoricalCrossentropy - multiclass classification with one-hot labels
- SparseCategoricalCrossentropy - multiclass classification with integer labels

***tf one-hot function:***
tf.one_hot(labels, depth=num_classes)

#### metrics
- mae/mse - regression / forecasting
- accuracy - classification


#### Save/Load model
- SavedModel - `model.save('SavedModel')`
- HDF5 model - `model.save('model.h5')`
- Load model - `loaded_model = tf.keras.models.load_model('filename')`

#### Download file from Google Colab
```
try:
  from google.colab import files
except ImportError:
  print("ImportError")
  pass
else:
  files.download('vecs.tsv')
  files.download('meta.tsv')
  print("Downloaded")
```