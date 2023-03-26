# Time-Series-Anomaly-Detection
Time Series Anomaly Detection LSTM Autoencoder in ECG Data

Time series anomaly detection using LSTM autoencoder in ECG data is a technique that involves the use of a specific type of deep neural network, known as a Long Short-Term Memory (LSTM) autoencoder, to identify abnormal patterns or outliers in electrocardiogram (ECG) data. The LSTM autoencoder is trained on a dataset of ECG signals to learn the normal patterns and then uses this learned knowledge to detect any deviations from the normal patterns in real-time. This method is particularly useful in identifying cardiac arrhythmias or other abnormalities that could be indicative of a heart condition. By detecting these anomalies early, medical professionals can take proactive measures to prevent or treat potential health issues.

# Autoencoder
Architecture d’un autoencoder:
Un autoencoder a une architecture très spécifique, car les couches cachées sont plus petites que les couches d’entrée. On appelle ce type d’architecture une architecture « bottleneck ». On peut décomposer un auto encodeur en deux parties à gauche et à droite de ce « bottleneck ».
La partie gauche s’appelle l’encodeur. L’encodeur transforme l’entrée en une représentation dans un espace de dimension plus faible appelé espace latent. L’encodeur compresse donc l’entrée dans une représentation moins coûteuse.
La partie droite est appelée décodeur, car elle doit reconstruire à l’aide de la représentation latente de l’entrée, une sortie la plus fidèle à l’entrée.

![illu_autoencoder_schema-19](https://user-images.githubusercontent.com/109078003/227786180-5c5c5869-4f3e-44e6-9e36-fa3a75a29161.png)

Lors de l’apprentissage, l’auto encodeur va donc apprendre à chercher à garder le plus d’information possible entre l’entrée et l’espace latent, afin que le décodeur ait les informations les plus essentielles pour reconstruire l’image. Ainsi, l’encodeur apprend les composantes les plus importantes d’une entrée pour avoir la meilleure compression possible.
