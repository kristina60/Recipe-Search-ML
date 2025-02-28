Recipe Generator using ML (TF-IDF & Cosine Similarity)

Overview

The Recipe Generator is a Django-based web application that helps users find recipes based on the ingredients they have. It uses TF-IDF (Term Frequency-Inverse Document Frequency) and Cosine Similarity to suggest the most relevant recipes. Users can input ingredients, and the system will return the first matching recipe based on similar ingredients. Additionally, users can search for recipes by name.

Features

- Ingredient-based Recipe Search: Users enter ingredients, and the system finds the closest matching recipe.
- Name-based Recipe Search: Users can search for recipes using their names.
- TF-IDF & Cosine Similarity Algorithm: The model calculates similarity between user-provided ingredients and stored recipe data.
- User-Friendly Interface: Simple and intuitive UI for easy interaction.

Technologies Used

- Python (Backend logic)
- Django (Web framework)
- Scikit-learn (For TF-IDF and Cosine Similarity computations)
- HTML, CSS, JavaScript (Frontend)

Installation & Setup

1. Clone the Repository:

   bash
   git clone https://github.com/kristina60/Recipe-Search-ML
   cd recipe-generator
   

2. Create a Virtual Environment:**

   bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   

3. Install Dependencies:

   bash
   pip install -r requirements.txt
   

4. Run the Development Server:

   bash
   python manage.py runserver
   

5. Access the Application:
   Open your browser and go to `http://127.0.0.1:8000/`

 How It Works

1. Preprocessing: The system processes recipe ingredients using **TF-IDF vectorization.
2. Similarity Calculation: When users input ingredients, the model computes the Cosine Similarity between user input and stored recipe data.
3. Recipe Recommendation: The system retrieves the first recipe with the highest similarity.
4. Search by Name: Users can search recipes directly by name using text matching.


## License

This project is licensed under the MIT License.

