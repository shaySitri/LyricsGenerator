# Song Generator using Deep Learning 🎶

[![Jupyter Notebook](https://img.shields.io/badge/Notebook-LFW_Siamese.ipynb-orange?logo=jupyter)](https://github.com/shaySitri/LyricsGenerator/blob/main/Lyrics_Generation.ipynb)

This project explores the exciting world of music generation using deep learning techniques. It leverages a dataset of song lyrics and corresponding MIDI files to build models that can generate new song lyrics inspired by musical characteristics.

## Project Overview 🎼

The goal of this project is to create models that can generate new song lyrics that are both coherent and musically inspired. To achieve this, the project employs deep learning models, specifically LSTM (Long Short-Term Memory) networks, that are trained on a dataset of song lyrics paired with their corresponding MIDI data.

## Steps involved in the project 👣

1. **Data Collection and Preprocessing 💽:**
   - A dataset of song lyrics and corresponding MIDI files was collected.
   - Lyrics were cleaned, tokenized, and converted into numerical representations.
   - MIDI files were analyzed to extract features such as song length, number of instruments, tempo, and piano roll.

2. **Model Development 🏗️:**
   - Two different LSTM models were developed:
      - **Model 1** incorporates MIDI features extracted from the songs, such as piano roll and chroma.
      - **Model 2** uses basic song statistics like length, instruments, tempo, and pitch distribution.
   - Both models were trained on the preprocessed dataset, aiming to capture relationships between lyrics and music.

3. **Model Evaluation and Generation 🧪:**
   - The trained models were evaluated using the BLEU score, a metric commonly used in machine translation to assess the quality of generated text.
   - Using the models, new song lyrics were generated based on input music or specific conditions.

## Packages used 📦

- **pretty_midi**: For analyzing and processing MIDI files.
- **matplotlib**: For data visualization.
- **pandas**: For data manipulation and analysis.
- **gensim**: For word embeddings and word2vec model loading.
- **seaborn**: For statistical data visualization.
- **nltk**: For natural language processing tasks like tokenization.
- **re**: For regular expressions to clean up the lyrics.
- **numpy**: For numerical computing.
- **sklearn**: For data preprocessing and model evaluation.
- **torch**: For deep learning model building and training.
- **tqdm**: For progress bars during training.

## Results ✨

The models were able to generate coherent song lyrics that exhibited some musical influence. However, there's room for improvement in terms of creativity and diversity. The BLEU scores, while not perfect, indicated a degree of similarity between generated lyrics and real lyrics.

## Future Directions 🚀

- Exploring more complex deep learning architectures such as Transformers or using bigger pre trained embedding.
- Incorporating melody and harmony features from MIDI files more explicitly.
- Experimenting with different lyric generation techniques, such as attention-based models.
- Adding parameters that will allow control over the generation process.

## Contributing 🤝

Contributions are welcome! Feel free to open issues or pull requests for any improvements or new ideas.
