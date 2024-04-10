# Guess the country "CAPITAL"

**pratice your geographical lesson by playing a little game.**
This repository contains a simple Express.js application designed to quiz users on world capitals. Users interact with the application through a web interface where they are presented with random countries and prompted to input the corresponding capital.

## Prerequisites
> Before running this application, ensure you have the following installed:
- Node.js
- npm (Node Package Manager)
- PostgreSQL

## Installation
1. Clone this repository to your local machine:
```bash
git clone https://github.com/therealmaduanusi/countryCapital
```

2. Navigate to the project directory:
```bash
cd <project-directory>
```

3. Install dependencies:
```bash
npm install
```

### Set up your PostgreSQL database:

- Create a database and a table named **capital**.
- Define the schema of the capital table with at least two columns: **country and capital**.

4. Create a .env file in the root directory of the project and define the following environment variables:

```plaintext
DB_USER=your_database_user
DB_HOST=your_database_host
DB_NAME=your_database_name
DB_PASSWORD=your_database_password
DB_PORT=your_database_port
```
## Usage
To start the application, run:
```bash
npm start
```
Once the application is running, access it through your web browser at http://localhost:4000 or 3000.

## Features
- **Quiz Interface**: Users are presented with random countries and prompted to input the corresponding capital.
- **Scoring**: Users receive immediate feedback on whether their answers are correct, and their total score is displayed.
- **Database Interaction**: The application interacts with a PostgreSQL database to retrieve a list of countries and capitals.

## Contributing
Contributions are welcome! If you find any issues or have suggestions for improvements, please open an issue or submit a pull request.

#### Code Snippets
```html
<button type="submit" id="submit">SUBMIT<% if(locals.wasCorrect){ %>
    <span class="checkmark">✔</span>
    <% } else if (locals.wasCorrect===false) { %>
        <span class="cross" id="error">✖</span>
    <% } %>
</button>
```
```js
res.render("index.ejs", { question: currentQuestion });
```


> [!IMPORTANT]
> The index file is now avaliable 😉.

> [!NOTE]
> Am still learning so please...😑.