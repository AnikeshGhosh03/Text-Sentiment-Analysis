# Text Sentiment Analysis with Caikit and Hugging Face

This project demonstrates how to perform sentiment analysis on textual input using a machine learning model served with **Caikit** and inference via a **gRPC client**. The model used is based on **Hugging Face transformers**, integrated with Caikit runtime for efficient deployment.

## 🚀 Features

- 📦 Model served using Caikit runtime
- 🧠 Uses Hugging Face sentiment analysis model
- ⚡ Inference through a gRPC client
- 💬 Accepts real-time user input from terminal
- 🔄 Easily extendable for other NLP tasks (e.g., summarization, NER)

## 📂 Project Structure

text-sentiment/
│
├── server.py # gRPC server serving the model
├── client.py # gRPC client that takes user input and gets sentiment
├── text_sentiment/ # Caikit data models
│ └── data_model.py
├── models/ # Pretrained Hugging Face model (optional)
├── requirements.txt # Python dependencies
└── README.md

yaml
Copy
Edit

## 🛠️ Setup Instructions

1. **Clone the repository**
   ```bash
   git clone https://github.com/AnikeshGhosh03/Text-Sentiment-Analysis.git
   cd Text-Sentiment-Analysis
Create and activate virtual environment

bash
Copy
Edit
python3 -m venv env
source env/bin/activate
Install dependencies

bash
Copy
Edit
pip install -r requirements.txt
🧠 Run the Project
1. Start the gRPC server
bash
Copy
Edit
python server.py
Leave this terminal running.

2. In another terminal, run the client
bash
Copy
Edit
python client.py
You’ll be prompted to enter a sentence.

The server will return the predicted sentiment.

✍️ Example
text
Copy
Edit
Enter a sentence for sentiment analysis (or type 'exit' to quit): I love working on this project!
RESPONSE: Sentiment = POSITIVE, Confidence = 0.98
📚 Dependencies
Python 3.8+

Caikit Runtime

gRPC

Hugging Face Transformers

Protobuf

🧠 About Caikit
Caikit is an open-source ML serving framework that simplifies building, training, and deploying models using gRPC interfaces. This project uses Caikit’s HuggingFaceSentimentTask module to run inference over gRPC.

🤝 Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

📄 License
Licensed under the Apache 2.0 License.

yaml
Copy
Edit

---

You can now **copy-paste this entire content into your `README.md` file** directly in your Cloud IDE. Let me know if you'd like to add author credits, demo screenshots, or badges.








Ask ChatGPT
