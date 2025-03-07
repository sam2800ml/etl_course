Dimensional model is the way that we organize the data, this is divided in two, facts or dimensiones the first emasurement like profit, and the second is the context like category or period
Star schema is because the nucleus is a table of facts and another table of dimensions with more context is mostly use for data warehouses, optimized for faster data retrieval, design for reporting/OLAP
is better organized, and the idea is to hav all the information in the database, and not use complex queries to be able to get to what youre tying to visualize.
Facts -> PK, FK, Facts
Dimensions -> /categorizes facts, supportive & descriptive, filtering, grouping and labeling, it helps us to organize everything, and do different opperations 
Snowflake schema it looks too organized but if you take a look into it, is very complex which if you are trying to analize the information you would have to do multiple joins to get to the right information, but everything depends on the project you are making, if you need to keep it simple whihc is faster to query and to analyze 


# Transformations
data cleaning, dealing with null values, duplicates
insert into the database, when we are going to add new ones, we put it under the first batch,
and update instead of increment we put the new ones on the position of the first batch
- Basic
    - Deduplication
    - Filtering
    - Cleaning and mapping
    - Value standarization
    - Key generation
- Advanced
    - Joining
    - Spliting
    - Aggregating
    - Deriving new values
- Data Cleaning
    - Handling missing values (imputation, deletion)
    - Removing duplicates
    - Standarizing formats
    - Correcting errors and inconsistencies
- Data Filtering
    - Removing irrelevant and unwanted data
    - Keeping only specific rows/columns based on conditions
- Data Aggregation
    - summarizing data
    - Computing averages
- Data Normalization
    - Scaling numerical values to a common range
    - categorical data into numerical form
- Data enrichment
- Data deduplication
- Data type conversion
    - Converting data types
- Key & index management
- Pivoting & unpivoting
- Splitting and merging columns
- Data masking & Anonymization

