# Semana 3
identificacion del problema y objetivo de los datos
Extraccion o captura de datos 100000 registros y minimo 10 columnas
Documento 
# Semana 6
transformaciones de los datos -> transformacion completa y adecuada de los datos, incluyendo cambio de formato y la eliminacion de duplicados o valores nulos
>
Preanalisis y visualizacion de datos -> analisis exploratorios de datos y visualizaciones avanzadas que revelan patrones claros usando EDA y matplotlib
>
# Rubrica final
Carga de datos en base de datos SQL -> carga eficiente de datos limpios en base de datos sql
Presentacion y storytelling de los datos -> Presentacion excepcional que utiliza tecnicas avanzadas de storytelling para comunicar insights de manera clara, atractiva y profesional

External databases that we want to move to stagging because its own by the company, then its move to the data warehouse so its accesible to transform it and work with that data organized, just connect to the data warehouse and procces it 

Databases
Can be a databases, files, web applications.
>
Etl its important because we have in there the volume  and that is the generated and kept, also the speed which the data is generated and is required to be extracted, and the variability of the formats and the type of availbale data

- Relational databases
    - its compose by tables, which have relations with another tables, we have primary key and foreign key, the last one is to identified the connection between one table to another table
- No relational dabases
    - Keep the data more flexible without having structure, those documents can be on JSON and also key and values
    vertcial, aumented of the resources addind more space on disk 500 gb -> 1 Tb
    horizontal, another instance, another server 
    - we use it when the database can change, 
- Plain files
    - Csv, json, parquet,xml.
    - Its simple to keep and to read, also high compability with different tools, can become insuficcient with big amount of data
- APIs
    - can communicate systems, and they use a protocol standarize, apirest uses the protocol HTTP to be able to do crud with the resources
- Data stream
    - systems and process data in real time, let you manage big volumes of continuos generated events
- Web Scraping
    - extract information directly on different web pages
- Logging and system events
    - The application normally generates events where those data can be monitor and diagnostic
- Iot sensors and real time data
    - the iot generated data in real time to be able to control and monitored


- Datamart
    - if the company have two different locations, or different process, we can use data mart to be able to keep the information for one city in one, and one for the other city, so people can only acces the one that they need 
- Staging
    - short  time on the source systems 
    - Quickly extract
    - Move the data into relational database
    - Start transformations from there
    - is the landing zone for our extracted data
    - data in tables and on a separate table
    - temporary  or persistent staging layers
- In-memory databases -> we use it when the price is no problem, when we need the data to be fast
    - Highly optimized for query performance
    - Good for analytics/ high query volume 
    - Usually used for data marts
    - Is faster because we dont have the latency 
    - if the memory losses energy everything will be lost 
    - We have to create a copy of the image, or create snapshot to be able to safe the information

- Row-based storage:
    - I the best suited fot OLTP
    - Works well with transactional worloads
    - Good for accesing entire records
    - Is easier to understand and work with for developers