# Sentiment-analysis-using-Gradio-interface
This project builds an interactive emotion and mental-health text classifier using pretrained Transformer models and deploys it through a clean, user-friendly Gradio interface.


It loads a pretrained GoEmotions model (SamLowe/roberta-base-go_emotions) to analyze and classify user input into fine-grained emotional categories like joy, sadness, anger, fear, love, and more.


It also loads a second transformer model (bhadresh-savani/distilbert-base-uncased-emotion), intended to estimate mental-health-related signals, though it actually functions as a general emotion classifier with categories such as anger, disgust, fear, joy, sadness, and surprise.


The notebook defines two prediction functions—one for detecting detailed emotions and another for identifying broader emotional or mental-state patterns. These functions handle tokenization, model inference, softmax scoring, and error management.



The app is launched using demo.launch(), allowing users to instantly test real-time classification of any text they provide.

A Gradio interface is created to make the system interactive, including a text input box, output fields for both emotion and mental-health categories, and JSON displays of class probabilities.



Finally, the notebook integrates both models into a single user interface, allowing users to type any sentence and instantly receive both emotional interpretation and mental-health-related label predictions in a simple, accessible web-based app.
