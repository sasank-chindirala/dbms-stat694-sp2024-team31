## Twitter Search Engine

This project presents a comprehensive exploration of data integration across diverse technologies, 
showcasing the seamless import of semi-structured twitter data into PostgreSQL and MongoDB databases. Complementing this 
integration is a powerful FastAPI-based search application, coupled with a frontend developed using React, enabling users to effortlessly retrieve data based on tailored queries. The project underscores the criticality of optimizing query efficiency through strategic caching mechanisms, employing Python dictionaries and advanced database indexing techniques. Through the implementation of search result caching and table indexing, significant reductions in query response times have been achieved, culminating in a more efficient and streamlined system. 

The `data-curation-application` directory has all the datafiles and code to build the databases used in this project.
The user and tweet databases and can be stored locally by using the `user-data-processor.ipynb` and `tweet-data-processor.ipynb` jupyter notebooks present in
the `non-relational` and `relational` sub-directories. The datafiles corona-out-2.zip and corona-out-3.zip are present
in the `data` sub-directory.


The code for the frontend React application can be viewed in the `frontend-application` directory. The application can be run as follows:
```
# To install the packages
npm i

# To start the frontend server
npm start
```

The code for the backend FastAPI application is present in `search.py` file in this project's root directory. Backend server can be started as shown below
```
# To install the required libraries
pip install -r requirements.txt

# To start the backend server
uvicorn search:app --port 8000
```

