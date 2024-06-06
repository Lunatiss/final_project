![Descripción opcional](img/_ (5).jpeg)

# Toward Sustainable Fashion?
> _A case study on ZARA's sustainability practices._
----

## 1. Libraries and Data used:
1.1 Libraries: <br>
    - selenium <br>
    - beautiful soap <br>
    - datetime <br>
    - pandas <br>
    - seaborn <br>
    - matplotlib <br>
    - numpy <br>
    - warnings <br>

## 2. Data source:
Web scraping on ZARA's website using selenium for dinamic webpage. Click here to see the raw data: [data/raw](data/raw)
For the scrip about web scrapping of Zara: [click here](notebook_web_scraping.ipynb) 
    

## 3. Data Cleaning Steps: 
Since the data was obtained through web scraping, the cleaning process was quite complex. 
Specifically, there was a column containing lists, which required special handling. We created a function to iterate over all the elements of these lists, access their components, transform them into strings, and then assign the relevant information to new columns:
**3.1. All the information was over Description Column (correponding on section view more in the web)**:
**Made_in**: Extracted the origin of the products from the description.
**Materials**: Separated the materials of the cloth such as cotton, polyamide, polyester, etc.
**Recycled Materials**: Further separated into categories like recycled cotton, recycled polyester, recycled polyamide, etc.
**Percentage Composition**: Assigned the percentage of each material's composition in accordance with each row.
**OCS and RCS**: Created columns for OCS (Organic Content Standard) and RCS (Recycled Content Standard) based on the descriptions obtained during scraping.
**Keep only necessary columns for analysis and change columns names.**

### 3.2 Keeping Necessary Columns and Renaming
- Only the necessary columns for analysis were retained and renamed for clarity and consistency.

### 3.3 Removing Duplicates and Empty Rows
- Duplicate values and empty rows were removed to ensure data integrity and accuracy.

### 3.4 Formatting Values
- Converted values to strings and numeric where appropriate.
- Removed spaces at the beginning and end of each string.
- Converted text to lowercase for uniformity.
- Removed punctuation marks specific to web scraping artifacts.
 

## 4. Visualization
4.1. Find visualization in Tableau: [Click here:](https://public.tableau.com/app/profile/luna.tissera/viz/Tableau_ZARA_2/Historia1?publish=yes) <br>


## 5. Analysis & Conclutions:




### Thank you!

