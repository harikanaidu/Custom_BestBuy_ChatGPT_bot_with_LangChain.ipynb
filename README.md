# Custom_BestBuy_ChatGPT_bot_with_LangChain.ipynb
Vector Document-based fine tuning of LLM using Chat-GPT's 3.5 turbo model and Langchain for memory

# Document Creation
The database consists of around 50 product details metadata entries named Sample BestBuy Product Entries consisting of the following parameters:
Category
Brand
Model Number
Warranty
Rating
Features
Description
Price

The database was in fact created bt prompt engineering ChatGPT as follows:
Hi You are a data-entry and database creator for a retail electronics store like BestBuy. You are now assigned a task to create metadata for 100 products listing the Category, brand, model number, warranty, rating, features, description and price as shown in the examples below. Please create metadata for 20 such products

1. Product: TechPro Ultrabook
   Category: Computers and Laptops
   Brand: TechPro
   Model Number: TP-UB100
   Warranty: 1 year
   Rating: 4.5
   Features: 13.3-inch display, 8GB RAM, 256GB SSD, Intel Core i5 processor
   Description: A sleek and lightweight ultrabook for everyday use.
   Price: $799.99

2. Product: BlueWave Gaming Laptop
   Category: Computers and Laptops
   Brand: BlueWave
   Model Number: BW-GL200
   Warranty: 2 years
   Rating: 4.7
   Features: 15.6-inch display, 16GB RAM, 512GB SSD, NVIDIA GeForce RTX 3060
   Description: A high-performance gaming laptop for an immersive experience.
   Price: $1199.99

This resulted in GPT outputting around 15 products, followed by passive persuasion and encouragement using prompts like...
"I knew you could do it. give me atleast 20 more unique products"

This process created a database of around 50 product features which will then be used to train the LLM.

# Training LLM



