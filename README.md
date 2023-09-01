# SmartParkingWeb
This project aims to recommend a free parking space to the user according to his/her destination. The destinatination time will differ from the time that free parking space is requested. Hence, a prediction algorithm is developed to satisfy the user.

This project is developed under GT-ARC, BeIntelli project, which is a smart car technologies project.

To reach the BeIntelli website, click the link => ['BeIntelli'](https://be-intelli.com/)

To reach the GT-ARC website, click the link => ['GT-ARC'](https://gt-arc.com/)

## Developer Documentation
The SmartParkingWeb is developed using:
- [FastAPI](https://fastapi.tiangolo.com/)
- [React JS](https://reactjs.org/)
- [Mongo DB](https://www.mongodb.com/)
- [Node JS](https://nodejs.org/)

### :file_folder:The layout of project folder/file structure
```
├── client
│   ├── public
│   ├── src
|   |   ├── components
│   │   ├── logos
│   │   ├── pages
│   │   ├── store
│   │   ├── App.js
│   │   └── index.js
│   └── package.json
├── backend
    ├── model.py
    ├── database.py
    ├── model.py
├── .gitignore
└── README.md
```
#### **Frontend side**
##### `client`- //This folder is for the frontend side of the application.
- ##### `public` - This holds all of our static files.
- ##### `src`- This holds all of the frontend react and javascript code files.
    - ##### `components` - This folder contains common design codes used in the application.
    - ##### `logos` - This folder holds the logos of clubs 
    - ##### `pages` - This folder contains individual subfolders of code for all pages used in the application.
    - ##### `store` - This folder contains the code that checks and handles if the user is logged into the app.
    - ##### `App.js` - This is what renders all of our browser routes and different views
    - ##### `index.js` - This is what renders the react app by rendering App.js
- ##### `package.json` - Defines npm behaviors and dependencies with packages for the frontend
#### **Backend side**
- ##### `config` - This holds our configuration files, like mongoDB configuration
- ##### `models` - This contains all of our data models for MongoDB
- ##### `routes` - This holds all of our HTTP to URL path associations for each unique url
- ##### `server.js` -This folder starts the backend application and provides a database connection.
- ##### `package.json` - Defines npm behaviors and dependencies with packages for the backend.Also includes first scripts to run the app
- ##### `.gitignore` - Tells git which files to ignore in Git
#### `README` - Informative documentation file of app
