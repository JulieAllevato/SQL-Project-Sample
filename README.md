### **New Wheels Sales Analysis (SQL Project Sample)**

---

### **Project Overview**
This project presents a comprehensive sales analysis for a fictional company, "New Wheels." The primary goal is to leverage SQL for data extraction and analysis to answer key business questions related to sales performance, product trends, and customer behavior. The project demonstrates skills in database design, data querying, and using the results for business intelligence.

---

### **Key Questions Addressed**
This analysis was designed to answer a series of business questions, including:
* Which products are the top sellers in terms of quantity and revenue?
* What are the monthly and quarterly sales trends over time?
* How does sales performance vary across different regions or sales personnel?
* What is the average order value, and how does it change over time?
* Who are the most valuable customers based on their purchase history?

---

### **Data Source & Schema**
The project is built on a relational database for a vehicle sales company. The database schema was designed to normalize and organize data efficiently.

* **Database Dump:** The `new_wheels_dumpfile.sql` file contains the schema and data to recreate the entire database.
* **Data Source:** The `new_wheels_sales.txt` file serves as the raw data used for populating the database.
* **Entity-Relationship (ER) Diagram:** An ER-Diagram (`ER-Diagram.pdf`) was created to visualize the relationships between the tables, demonstrating a foundational understanding of database design.

---

### **Methodology & Tools**
The project follows a rigorous data analysis workflow centered around SQL:

1.  **Database Design:** An ER-Diagram was created to model the relationships between tables (`Customers`, `Products`, `Sales`, etc.).
2.  **Data Loading:** SQL was used to create the database schema and load the raw data into the respective tables.
3.  **Advanced Querying:** Complex SQL queries (`Project Solutions.sql`) were written to aggregate data, join multiple tables, and extract key insights to answer the business questions.
4.  **Reporting:** The results of the SQL queries were exported and used to create visualizations and a final report (`FINAL PROJECT SOLUTIONS- Allevato.pdf`).

**Tools Used:**
* **SQL:** For database design, data loading, and all analytical queries.
* **Excel:** For creating visualizations and charts from the query results.
* **PDF:** For documenting the database schema and final project solutions.

---

### **Visualizations & Findings**
The analysis resulted in several key findings, presented through visualizations to make them easy to understand.

* **Q1: Find the total number of customers who have placed
orders. What is the distribution of the customers across states?**

<img width="772" height="233" alt="image" src="https://github.com/user-attachments/assets/36133fbc-4a1b-46ce-9416-efbb6b9e1ab7" />

     Caption: This chart shows the total number of customers and the distribution of customers across states.

* **Q2: What are the top 5 vehicle makers preferred by the customers?**
  
<img width="417" height="243" alt="image" src="https://github.com/user-attachments/assets/e870286c-a95e-47ca-9e54-9e52720fe991" />
    
    Caption: A pie chart detailing the most popular vehicle makers preferred by customers.
    
* **Q3: Which is the most preferred vehicle maker in each state?**

<img width="685" height="780" alt="image" src="https://github.com/user-attachments/assets/f4b1a3bf-3cf3-4b8f-9198-0088bae5f104" />

    Caption: A map visualizing preferred vehicle maker in each state.
      
* **Q5: Find the percentage distribution of feedback from the customers. Are customers getting more dissatisfied over time?**

<img width="641" height="424" alt="image" src="https://github.com/user-attachments/assets/02a54b48-f019-4420-ba2f-04321588e3fb" />

    Caption: A 100% bar chart showing increasing customer dissatisfaction by quarter.
      
* **Q6: What is the trend of the number of orders by quarter?**

<img width="662" height="441" alt="image" src="https://github.com/user-attachments/assets/3319b280-523f-4cda-b797-1058b6e67414" />

    Caption: A bar chart showing the trend of sales per quarter.
      
* **Q8: What is the trend of net revenue and orders by quarters?**

<img width="628" height="682" alt="image" src="https://github.com/user-attachments/assets/fd38c027-5dba-4de2-a432-87ed16cdf43c" />

    Caption: A visualization of the declining trend of net revenue and orders by quarter.
      
* **Q10: What is the average time taken to ship the placed orders for each quarter?**

<img width="441" height="268" alt="image" src="https://github.com/user-attachments/assets/4dc27b85-8986-4465-a7ad-da43d86e665c" />

    Caption: A table showing the customer rating decreasing as average ship time increases per quarter.
      

---

### **Business Metrics Overview**
<img width="656" height="130" alt="image" src="https://github.com/user-attachments/assets/188b7c6e-a7b9-4eb9-96af-1c03f248f5ac" />

    This overview displays **total revenue, total orders, total customers, average customer rating** and other key metrics.

---

### **Business Recommendations**
* The decrease in customer satisfaction correlates strongly with increased shipping times. This could lead to a **10-15% churn rate among dissatisfied customers**. I recommend an investigation into the logistics of these 'bad' shippers, as this could save the company in lost revenue from customer churn.
* **35% of your customer base (349 out of 994)** comes from California, Texas, Florida, and New York. I recommend offering a sale to draw in more customers from those four key states.
* The most popular vehicle makers in those states were **Audi in California, Chevrolet in Texas, and Toyota in New York and Florida**. A sale on those makers would likely bring in a larger client base during the promotion.
* New Wheels received only "Very Bad" or "Bad" feedback when shipping orders through the following shippers:
  * Realcube, Meembee, Livefish, Shuffletag, Myworks, Cogibox, Buzzdog, Jatri, Aibox, Gigaclub, Mita, Fliptune, Dynava, Dynazzy, Jaxbean, Shufflebeat, Vitz, Babblestorm, Fivechat, Flipstorm, Blogpad, Skinder, Twitterbridge, Flashset, Bluezoom, Tanoodle, Browsezoom, Fatz, Topiclounge, Aimbo, Ntags, Skyndu, Meedoo, Tavu, Rhybox, Npath, Tambee, Meemm, Dabjam, Jabbertype, Tekfly, Mudo, Demivee, Voolith, Yoveo, and Demimbu.
**Further analysis could involve creating a stored procedure to automatically flag orders being shipped by 'bad' shippers.**
