# AI Chatbot using Deep Learning and Natural Language Processing
**Created by:** Saanchi Jalewa  

This project is an **intent-based AI chatbot** built using **Natural Language Processing (NLP)** techniques and a **Deep Learning model** in PyTorch, with a **Flask** backend for serving responses.  

---

## 📌 Features
- **Intent Recognition:** Understands user queries based on trained intents.
- **NLP Preprocessing:** Uses tokenization, stemming, and Bag of Words (BoW) for text processing.
- **Deep Learning Model:** Feedforward Neural Network (FNN) for intent classification.
- **Flask API:** Simple REST endpoint to connect backend and frontend.
- **Customizable Training Data:** Modify `intents.json` to train the chatbot for new topics.

---

## 🚀 How It Works
1. **Data Preparation**  
   - Define user inputs and matching intents in `intents.json`.  
   - Example:
     ```json
     {
       "tag": "greeting",
       "patterns": ["Hi", "Hello", "Good day"],
       "responses": ["Hello!", "Hi there!", "Greetings!"]
     }
     ```

2. **Data Preprocessing**  
   - Tokenize and stem words.
   - Create Bag of Words for model training.

3. **Model Training**  
   - Train an FNN model using PyTorch.
   - Save the trained model for later use.

4. **Flask Integration**  
   - The chatbot’s predictions are served via a `/predict` API endpoint.

---

## 🛠️ Installation & Setup

### 1️⃣ Clone the repository
```bash
git clone https://github.com/saanchi-jalewa/Chatbot.git
cd Chatbot
```

### 2️⃣ Create a Virtual Environment
```bash
python -m venv venv
venv\Scripts\activate  # For Windows
# OR
source venv/bin/activate  # For Mac/Linux
```

### 3️⃣ Install Dependencies
```bash
pip install -r requirements.txt
```

### 4️⃣ Download NLTK Data
```bash
python
>>> import nltk
>>> nltk.download('punkt')
```

### 5️⃣ Train the Model
```bash
python train.py
```

### 6️⃣ Run the Chatbot (Terminal)
```bash
python chat.py
```

### 7️⃣ Run Flask API
```bash
python app.py
```
Open [http://127.0.0.1:8000](http://127.0.0.1:8000) in your browser.

---

## 🧠 Technologies Used
- **Python**
- **PyTorch**
- **NLTK**
- **Flask**
- **JSON** (for intents data)

---

## 📄 License
This project is open-source and free to use for learning purposes.
