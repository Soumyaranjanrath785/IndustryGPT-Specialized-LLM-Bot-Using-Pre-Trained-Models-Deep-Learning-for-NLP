# IndustryGPT-Specialized-LLM-Bot-Using-Pre-Trained-Models-Deep-Learning-for-NLP

The major components of this project include dataset collection, data preprocessing, model selection, fine-tuning, deployment, and chatbot development. Finance-related datasets were collected from Hugging Face, including Finance Alpaca 1K Test and Alpaca Finance EN. The collected data was cleaned, organized, and reformatted into the TinyLlama instruction template format for supervised fine-tuning. The pre-trained model used in this project was TinyLlama-1.1B-Chat-v1.0, chosen because of its lightweight architecture and efficient performance on limited GPU resources.

To optimize training efficiency, advanced fine-tuning techniques such as PEFT, LoRA, and QLoRA were implemented. QLoRA enabled 4-bit quantized training, significantly reducing GPU memory usage while maintaining model performance. The model was fine-tuned using Google Colab T4 GPU with optimized training parameters, gradient checkpointing, and BitsAndBytes quantization.

After training, the fine-tuned model and tokenizer were saved and uploaded to the Hugging Face Hub for easy access and deployment. A Flask backend API was developed to handle chatbot requests and generate responses using the TinyLlama model. ngrok was used to expose the Flask server publicly, allowing the chatbot API to be accessed online. A Streamlit-based frontend interface was also developed to provide a user-friendly chatbot interaction system.

Finally, the chatbot was tested with finance-related questions to evaluate its conversational ability, contextual understanding, and response generation performance.
