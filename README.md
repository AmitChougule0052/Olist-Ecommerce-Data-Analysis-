# Olist-Ecommerce-Data-Analysis-
Data Analytics :- Olist Ecommerce Data .


# Olist Store Analysis : 

## Introduction : 

Olist is a Brazilian e-commerce platform that connects small and medium-sized businesses to customers across Brazil. The platform operates as a marketplace, where merchants can list their products and services and customers can browse and purchase them online.The dataset is designed to help analysts and researchers better understand the e-commerce landscape in Brazil and identify opportunities for growth and optimization. To help Olist gain better insights into its e-commerce platform and optimize available opportunities for growth,we will perfom some KPI's and answer some business questions,thereby providing Insights and recommendations.

## Data Discription : 

The features allow viewing orders from multiple dimensions: from order status, price, payment, and freight performance to customer location, product attributes, and finally reviews written by customers. For this challenge, I used MySQL to access the dataset, clean and perform Data Analysis using BI tool Tableau.

Below is the outline of the challenge

• Explore Dataset and perform Data Validation
• Data Cleaning
• Perform KPI's Data Analysis
• Share Insights and Make recommendations

## Data Schema : ![WhatsApp Image 2025-05-29 at 12 58 04 PM](https://github.com/user-attachments/assets/d7ef6fcb-f127-4b0f-b5bc-785794cd81a0)
























## Data Explorationh And Validation : 

 I Explored 9 different tables with the excel and from this process , i discovered the dataset had the following quality issues : 

    • Null and the Empty values 
    • Unwanted Speecial characters 
    • Irrelevent columns .
    • Errors in the Spelling . 


## Data  Cleaning : 

  In the data cleaning i used the MySQL 

  • Converting and the updating the translation table. There are the rocords in the category column that requires us to replace with the english translated versions of the Portuguese strings from the category_name_translatn table, but after confirmng the distinct records from the translation table. 





![b805f8a9-9865-41fa-9d37-ed7e2eb93f39](https://github.com/user-attachments/assets/0a2fce9c-738a-42d7-8b30-f44fd84259ff)









  •  Deteting the unwanted attributes/ Columns for the optimized analysing and reducing the time. 

  • Check the null records and replace them with the correct strings or numeric values after checking for the null values , there are 610 records with the null values in the category , name_length , descriptn_len   , and photos_qty columns of the products table. i used the coalesce function to replace the null values in the category with N/A , and 0 with the null values in the name_length , descriptn_len , and photos_qty 
    columns. 






![ae96de23-354d-4049-8fa7-b18b8462b7f6](https://github.com/user-attachments/assets/0fbcbe76-bcfb-4a1d-b730-5882ea8c730a)






## Perform KPI's Data Analysis : 

1. Weekdays vs Weekend (Order_purchase_timestamp) payment statistics .



![280260ff-64dc-4f1f-b5eb-4546480d4e9b](https://github.com/user-attachments/assets/1fc4f091-a0cb-4f30-8464-6f42c779cb9f)








![39d5c472-d252-474e-a991-43ee71c64e55](https://github.com/user-attachments/assets/f8d55d22-dcf1-4054-8f55-31aa65b60d68)









## 2. Nukmber of the orders with review score 5 and payment type as credeit card. 











