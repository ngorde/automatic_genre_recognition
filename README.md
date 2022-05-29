# Automatic genre recognition

This work is about automatic genre recognition.

We propose several models classifying songs into 8 genres: pop, rock, r&b, hip-hop, country, folk, blues, and jazz.

We used a bi-directional LSTM network, BERT, a model trained on audio features from Spotify, and an ensemble of neural networks including it and LSTM.

The data for training and testing was two corpuses of English-language songs, which were compiled from material primarily from resources such as Spotify. Genius and Rate Your Music.

The genre-balanced corpus contained the lyrics and musical attributes of more than 8,000 songs, and the unbalanced corpus contained more than 10,000 songs.

We got a fairly high F1-measure of genre detection at 8 classes. Models trained on the genre-balanced corpus were generally better in their performance. In terms of text analysis, the BERT model performed best, but the LSTM model trained on our data also performed well with a simpler architecture and fast training. 

The metadata of musical attributes from Spotify was enough to build a fairly high-quality recognizer, while the ensemble with a neural network analyzing text properties showed no significant advantage.
