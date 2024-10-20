# Cornell-Movie-Dialog-Corpus

# Final Team Project: Cornell Movie Dialog Corpus

## Overview
This project aims to create an AI-powered chatbot capable of interacting with users to provide information about movies, including recommendations, plot details, and general movie trivia. Our chatbot is built using a fine-tuned GPT-2 model, trained on the Cornell Movie Dialogues dataset, and employs fallback strategies to ensure coherent responses. This project was completed as part of our graduate program's final requirement for the AAI 520 course.

## Features
- **Conversational Movie Recommendations**: Users can interact with the bot to receive personalized movie suggestions, particularly for specific genres or occasions.
- **Movie Information**: The bot can provide information about movie directors, plot summaries, and general trivia about popular movies.
- **Fallback Strategy**: For questions where the bot struggles to generate a coherent response, a fallback mechanism was designed to provide a sensible default reply or escalate to re-generating a response.
- **Evaluation Metrics**: Responses are evaluated based on Perplexity as the metric. to ensure conversational quality.

## Dataset
We used the **Cornell Movie Dialogues dataset** consisting of movie dialogue scripts to train our model. This dataset contains conversational exchanges between movie characters, offering a wide variety of movie-specific conversational contexts.

## Model Details
- **Model Architecture**: The chatbot utilizes a **GPT-2 model**, which has been fine-tuned on our specific dataset to improve response quality in the movie recommendation and trivia context.
- **Training Setup**: The model was trained using Google Colab with an L4 GPU to accelerate the training process.
- **Fine-tuning**: We experimented with different hyperparameters, including learning rate and batch size, to achieve an optimal balance between creativity and coherence.

## Key Challenges
- **Resource Limitations**: Managing GPU and computational resources posed a significant challenge due to the size of the dataset.
- **Response Consistency**: Ensuring that the generated responses are relevant and informative required multiple iterations in the training process. Fallback strategies were incorporated to handle incoherent responses.

## Installation and Setup
To run the chatbot on your local machine:
1. Clone the repository:
   ```bash
   git clone https://github.com/AryazRez/Cornell-Movie-Dialog-Corpus.git
   ```
2. Download the pretrained GPT-2 model and move it into the appropriate directory.
3. Run the pre-processing and fine-tuning notebook:
   ```bash
   AAI-520_Final_Project_AAZ.ipynb
   ```
4. Save and move fine-tuned model to appropriate directory.
5. Run the chatbot notebook and begin asking questions in Tkinter chatbot:
   ```bash
   AAI-520_Final_Project_Chatbot.ipynb
   ```

## Usage
Upon running the script, users can interact with the chatbot directly from the terminal. The bot will answer questions influenced the trained movie scripts

## File Structure
- **AAI-520_Final_Project_AAZ.ipynb**: Data pre-processing and model fine-tuning
- **conversation_pairs.csv**: Preprocessed dialogue dataset used for model fine-tuning.
- **AAI_520_Final_Project_QA.ipynb**: Imported fine-tuned model that contains basic Q&A chatbot.
- **AAI_520_Final_Project_Chatbot.ipynb**: Notebook that contains Tkinter GUI for chatbot.

## Evaluation Metrics
- **Perplexity**: Measures the fluency, predictability, and certainty of the model's responses.

## Future Improvements
- **Model Expansion**: Exploring the use of larger models such as GPT-3 to enhance conversational depth.
- **Enhanced Fallback Mechanism**: Improve fallback responses using more advanced techniques for sentiment detection and user intent classification.
- **Web Interface**: Develop a web-based interface for easier user interaction beyond the command line.

## Contributing
We welcome contributions to improve the chatbot. Feel free to create a pull request or open an issue for any suggestions.

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgements
- Our team members for their invaluable collaboration and dedication throughout the project.
- The Cornell Movie Dialogues dataset creators for providing an engaging dataset for model training.
- Faculty members and mentors from our graduate program for their guidance.
