# chaabi_
this repo contains the api for the chaabi assignment 

# installation guide
Installation Guide:

**Step 1:** Install the required dependencies mentioned in the `requirements.txt` file using the command:
```bash
pip install -r req.txt
```

**Step 2:** Download the following pickle files:
1. **"Collection.pkl"**
   - This file includes the Qdrant client, facilitating the retrieval of relevant context/documents from the database for a given question.
   
2. **"embedding_model.pkl"**
   - This file contains the sentence transformer, utilizing the "multi-qa-MiniLM-L6-cos-v1" model for embedding.

3. **"Reader.pkl"**
   - This file includes the pipeline responsible for processing questions and extracting answers.

**Step 3:** Run the Python file `app.py` to utilize the API model. Execute the following command:
```bash
python app.py
```

This repository includes the API file for the chaabi assignment, along with an installation guide for the setup process. Here are some examples of queries and their corresponding answers:

1. **Query:** What is the best cream for the face?
   - **Output:** Garnier BB Cream for women
   - **Prediction Score:** 0.4385122060775757
   - **Referred Product:**
     - Product Name: Skin Naturals - BB Cream
     - Category: Beauty & Hygiene
     - Sub_Category: Makeup
     - Brand: Garnier
     - Type: Face
     - Market Price: 165.0
     - Sale Price: 123.75
     - Rating: 4.1

2. **Query:** What is the best-rated hair product?
   - **Output:** 4.2
   - **Prediction Score:** 0.8899042010307312
   - **Referred Product:**
     - Product Name: Advanced Hair Fall Solution Shampoo - Silky Smooth Care
     - Category: Beauty & Hygiene
     - Sub_Category: Hair Care
     - Brand: Pantene
     - Type: Shampoo & Conditioner
     - Market Price: 60.0
     - Sale Price: 60.0
     - Rating: 4.2

3. **Query:** Which is the best cream for dry skin?
   - **Output:** Shea Smooth Body Lotion
   - **Prediction Score:** 0.4244949221611023
   - **Referred Product:**
     - Product Name: Shea Smooth Body Lotion for Dry Skin - Men & Women
     - Category: Beauty & Hygiene
     - Sub_Category: Skin Care
     - Brand: Nivea
     - Type: Body Care
     - Market Price: 425.0
     - Sale Price: 300.0
     - Rating: 4.2

4. **Query:** Price of Dove soap?
   - **Output:** 149.0
   - **Prediction Score:** 0.5285995602607727
   - **Referred Product:**
     - Product Name: Bathing Soap - with Neem, Tulsi & Aloe Vera
     - Category: Beauty & Hygiene
     - Sub_Category: Bath & Hand Wash
     - Brand: Hamam
     - Type: Bathing Bars & Soaps
     - Market Price: 149.0
     - Sale Price: 149.0
     - Rating: 4.4

5. **Query:** Suggest a healthy snack.
   - **Output:** Whole grain oats help improve your heart health
   - **Prediction Score:** 0.27581632137298584
   - **Referred Product:**
     - Product Name: Chips - Cheese & Jalapeno
     - Category: Snacks & Branded Foods
     - Sub_Category: Snacks & Namkeen
     - Brand: RiteBite Max Protein
     - Type: Namkeen & Savoury Snacks
     - Market Price: 120.0
     - Sale Price: 120.0
     - Rating: 4.0

6. **Query:** Can you give the rating of Dettol soap?
   - **Output:** 4.3
   - **Prediction Score:** 0.9303156733512878
   - **Referred Product:**
     - Product Name: Bathing Bar Soap - Cool
     - Category: Beauty & Hygiene
     - Sub_Category: Bath & Hand Wash
     - Brand: Dettol
     - Type: Bathing Bars & Soaps
     - Market Price: 330.0
     - Sale Price: 280.5
     - Rating: 4.3
