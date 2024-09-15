Key Highlights of the Project:
Character-Based Model Using GRU:
I built an RNN model that generates text character by character. The model uses a GRU layer with stateful=True to maintain the state between batches and generate coherent sequences.

Character-to-Index Mapping:
I transformed characters into numerical representations using a char2idx mapping and fed them into an Embedding layer to convert characters into vector form for the model.

Training with Checkpoints:
During training, I saved the model's weights using ModelCheckpoint, allowing me to reload the weights and continue generating text seamlessly.

Generating Text Dynamically:
The model generates text based on a user-provided start string. By adjusting the temperature, I was able to control the randomness and diversity of the generated text, resulting in creative and unique outputs.

Optimizing Batch Size and Weights Loading:
I overcame challenges related to batch size while using stateful=True in the GRU layer and successfully restored the saved weights without errors.

🔧 Technologies Used:

TensorFlow & Keras
GRU Networks for Text Generation
Character-Level NLP
Weight Saving and Restoration for Reusability
💡 What’s Next?
I’m planning to further improve the model by exploring attention mechanisms and experimenting with even more sophisticated architectures to enhance the quality of the generated text.
