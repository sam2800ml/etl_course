# ETL
The main thing, would be to extract the data, transform it, and then load it to data warehouse so it can be analysed after, his can be done visualize to implement a better analysis on the data, like insights, kpis,

## File format
the files formats is a really important part for what we doing, this is because of the following:
- Large data storage = High costs
- Long read/writes times = Slow systems, high computational power
- High computation power = increased in cost
> 
Thats why when we are choosing our file format we have to selct the one that fit us best depending on the project that we are working some of the file formats that exist and some people is using are the followings:
-   XML: is a text-based file format for storing and exchanging structured data, uses tags to define elements and attributes their properties, is the least efficient file format
>
- Parquet: Is a column-oriented file format developed for big data processing, it is designed to store and retrieve data efficiently by partitioning and compressing columns of data, it is suitable for large datasets and supports complex data types, but not everyone can use it, its necesarily to use an especialized software to be able to work with it, and its the fastest
    - Advantages:
        - Suitable for partitioned data
        - Small file size
        - Fastt read operations
        - Supports nested data
        - Stores data types
        - Ideal for large datasets
    - Limitations:
        - Cannot be read with text editors
        - Limited support outside Apache Spark and Apache Hadoop
        - Requires specialized knowledge

>
- Feather: is a lightweight and efficient format for storing data frames, also like the previous stores the data in binary format, making it smaller and faster to read and write.
>
- CSV: its the most used in the industry, and is for storing and exchanging tabular data, cannot store complex data types, issues with special characters, distinguishing betweem null and blank values, is row oriented which makes it slower.
    - Advantages:
        - Easy to understand
        - Small file size
        - can be opened and edited with text editors
        - Widely supported
        - Suitable for small datasets
    - Limitations:
        - Does not store data types
        - cannot store complex data
        - Not suitable for large datasets
        - so support for null and blank values
        - Not suitable for patitioned data storage
>
- JSON: is also a lightweight and versatile format to storing and exchanging structured data, uses the key and value pair to represent data objects, its not in good use for large and complex datasets as can be very difficult to read, takes a long time to read, is row oriented, which makes it take a lot of time to query
    - Advantages:
        - Readable and undestandable
        - support complex data structures
        - can be opened and edited with text editors
        - Widely supported
        - Suitable for data object exchange
    - Limitations:
        - Requires transformation to tabular format for RDBMS storage
        - cannot validate schemas
        - Larger file size compared to CSV and Parquet
        - so support for null and blank values
        - Not suitable for patitioned data storage
>
- Avro: Stores metadata as JSON, making it readable, supports schema changes well and performs serializarion efficiently, the data is serialized


Etl with agents?
we can extract the characteristics from the database, after we collect those items we can transform them, and we start to prepared all the items so we can show them, and can let it be freely to used by anyone that needs that information 

- Data warehouse: Storing digital transformation in a manner that is secure, reliable, easy to retrieve and easy to manage, all the items are organized depending of the use of them, in this warehouse we just keep al the information organized, is to keep all the information that is going to give us a value for the bussiness, this only saves rhe information that is needed, the data is segmented, those are the same databases but with some differents characteristics, user friendly, fast consultation, easy data analysis, al the data is centralized in the data warehouse:
    - Analytical decision making (OLAP): improve the decisions, is faster because we have everything organized and already to be used
    - Operational data keeping (OLTP): is in the moment, all the data that is for the bussiness and move the parts fundamental 
    - Steps in a data warehouse:
        - Data soucers
        - staging: make sure that the data is safe, in case that some of the apis of the providers stops working, we have the raw data, and when we want to keep it, we transform it, and then load it 

- Data lake: is a place where  we safe some files, can be structured data, unstructured like media files, semi structured like word, JSON, this is kept on the data lake, and the purpose is to be a place where the data exist 

data Govern: Data security, privacy and access, discovery logs, Classification, Lineage, Quality and standards, Regulations and compliance

Operate: Monitor, Logging, Alert, Backup and restore, Archive, Replicate, Disaster Recovery



bibliography
- https://medium.com/@aiiaor/which-data-file-format-to-use-csv-json-parquet-avro-orc-e7a9acaaa7df
- https://medium.com/@gadhvirushiraj/the-best-file-format-for-data-science-ed756f937be8
