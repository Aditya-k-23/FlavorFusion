# FlavorFusion

An AI-powered recipe recommender.

## Data

The data used in this project is from the [Food.com dataset](https://www.kaggle.com/shuyangli94/food-com-recipes-and-user-interactions). The dataset contains 180K+ recipes and 700K+ recipe reviews.

## System Architecture

![System Architecture Diagram](https://github.com/AnaqiAmir/FlavorFusion/blob/009037774e33a247e6deafba4f0cb48d374290dd/assets/system_architecture.png)

- **User Interface (UI)**:
  - **Function**: Collects user inputs (preferences, nutritional needs, allergens, etc.) and displays recommendations.
  - **Tools**: Web interface (React/Flask/Django), chatbot (Rasa/Dialogflow).
- **Natural Language Understanding (NLU)**:
  - **Function**: Understands user inputs and extracts relevant features like nutritional requirements, preferences, allergens, etc.
  - **Tools**: OpenAI GPT-4 (or similar LLM), Hugging Face Transformers, spaCy.
- **Feature Extraction**:
  - **Function**: Converts extracted user requirements into structured features for recommendation.
  - **Tools**: Preprocessing pipelines (Pandas, NumPy), LLM fine-tuning or embeddings.
- **Recipe Matching (kNN-based Recommender)**:
  - **Function**: Identifies recipes that best match user preferences and nutritional requirements.
  - **Tools**: Scikit-learn for kNN, custom ranking logic for dietary requirements.
- **Validation Model**:
  - **Function**: Validates and fine-tunes recommendations for user-specific needs.
  - **Tools**: Gradient Boosting/Random Forest (Scikit-learn), Neural Networks (PyTorch/TensorFlow).
- **Database**:
  - **Function**: Stores the food.com dataset, user preferences, and recommendation results.
  - **Tools**: PostgreSQL/MySQL, MongoDB (for NoSQL flexibility).
- **APIs**:
  - **Function**: Communicates between the backend recommendation engine and the UI.
  - **Tools**: FastAPI, Flask.
- **Evaluation and Feedback Loop**:
  - **Function**: Captures user feedback and adjusts future recommendations.
  - **Tools**: Reinforcement learning, A/B testing frameworks.

## ✍️ Authors

- **Aditya Kulkarni**

  - LinkedIn: [@aditya-s-kulkarni](https://www.linkedin.com/in/aditya-s-kulkarni/)
  - GitHub: [@Aditya-k-23](https://github.com/Aditya-k-23)
  - Website: [adityakulkarni.me](https://adityakulkarni.me)

- **Anaqi Amir**
  - LinkedIn: [@anaqi-amir](https://www.linkedin.com/in/anaqi-amir/)
  - GitHub: [@AnaqiAmir](https://github.com/AnaqiAmir)
