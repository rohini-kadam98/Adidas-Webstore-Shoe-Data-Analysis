# Adidas Webstore Shoe Data Analysis
### Tool Used
Microsoft Power BI

### Data Used
country_dim, shoes_dim, shoes_fact

## About Data
### country_dim 
Contains country codes, currency, and shoe measurement metrics.
### shoes_dim 
Contains shoe details, including ID, name, best use case, gender, color, and image URL.
### shoes_fact
Contains transaction-level data, including shoe ID, price, category, size, availability, date, and country code.

### Data Cleaning & Transformation:
Ensure date columns are in Date format.
Convert price to currency format.
Remove any unnecessary columns like Unnamed: 0 in shoes_fact.

### Create Relationships
shoes_fact.id → shoes_dim.id (One-to-Many)
shoes_fact.country_code → country_dim.country_code (Many-to-One)

### Key Performance Indicators (KPIs)
Total Revenue = SUM(shoes_fact[price])
Total Sales = COUNT(shoes_fact[id])
Average Price = AVERAGE(shoes_fact[price])
Stock Count = SUM(shoes_fact[availability])
Stock Count = SUM(shoes_fact[availability])

![Dashboard](https://github.com/rohini-kadam98/Adidas-Webstore-Shoe-Data-Analysis/blob/main/Adidas%20Webstore%20Dashboard.png)

### Key Insights
I recently worked on an Adidas Webstore Shoe Data Analysis to uncover key business insights. Here are key findings:              
1️⃣ The webstore has generated $30M in total revenue with 299K total sales, indicating strong business performance.                        
2️⃣ Germany leads the market, generating $20.8M in sales, far ahead of other countries.                        
3️⃣ Core Black is the most popular shoe color, with 10M+ sales.                                                           
4️⃣ Revenue peaked in January ($6.3M) but saw a decline in the following months.                                                       
5️⃣ Tensaur Hook and Loop is the top-selling shoe, selling 6.2K units.                                                                        
6️⃣ Running shoes dominate sales, contributing 37.72% of total revenue.                                                                                    
7️⃣ Since running shoes are the most popular category, Adidas can expand its product line or enhance marketing efforts for this category.                                   
8️⃣The UK has the lowest sales (only $0.2M), showing potential for market expansion.                                                                             

Thank you for reading and evaluating my repo :)
Live Dashboard [Link](https://app.powerbi.com/view?r=eyJrIjoiOGFhNTU5OWEtZDk3MS00YjQ4LWIxMTEtYmVjOTlmOTkzNWZmIiwidCI6ImM2ZTU0OWIzLTVmNDUtNDAzMi1hYWU5LWQ0MjQ0ZGM1YjJjNCJ9)
