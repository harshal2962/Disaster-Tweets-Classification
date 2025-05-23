🌪️ NLP for Disaster Tweet Classification
Can AI save lives? This project uses Natural Language Processing (NLP) to classify tweets as real disaster alerts or irrelevant content?
Built on BERT for bidirectional context understanding, the model helps emergency services filter signal from noise on social media in real time.

🚨 Problem Statement
In the early moments of a disaster, Twitter is often the first source of information—but it's cluttered with sarcasm, humor, and false alarms. Misclassifying these tweets can lead to:

>Panic due to false positives

>Missed responses to real disasters

>Spread of misinformation by news or public agencies

>This project aims to solve that by classifying tweets as either:

>✅ Real Disaster: "Massive earthquake hits Japan. 7.5 magnitude."

>❌ Not a Disaster: "My phone died… total disaster 😩"

🧪 Models Compared
Model           	Accuracy	   Comments-
>Regression      	66–68%	     Fails on context & sarcasm
>Neural Network	  73%	         Misses word sequence understanding
>BERT	            F1 = 0.82	   Best for contextual understanding, but resource-heavy

🤖 Why BERT?
>📌 Handles negation & sarcasm effectively

>📌 Uses self-attention to consider word order and context

>📌 Processes tweets bidirectionally, unlike traditional models

>✅ Identifies phrases like “not a disaster” vs. “total disaster” with high precision

⚙️ How BERT Works (Simplified)
>Tokenization into subwords

>Special tokens like [CLS] and [SEP]

>Word & positional embeddings

>Self-attention over entire sequence

>Contextual sentiment/negation learning

>Final classification → Disaster or Not

🧰 Tech Stack
>Python, Pandas, Sklearn, PyTorch

>HuggingFace Transformers (BERT, DistilBERT)

>Jupyter Notebooks

>Dataset: 10,000 labeled tweets from Kaggle

📂 Project Structure
.
├── data/                    # Labeled tweet dataset
├── preprocessing/           # Cleaning & tokenization scripts
├── models/                  # BERT and baseline models
├── notebooks/               # EDA and experimentation
├── README.md
└── requirements.txt

🧠 Key Takeaways
>BERT achieves superior classification through transfer learning and contextual awareness.

>False disaster tweets are filtered, helping emergency services prioritize real-time responses.

>Future work: Real-time deployment using DistilBERT, mobile integration for field agents.

👤 Author
Harshal Amin
📍 MSBAIM, Purdue University
