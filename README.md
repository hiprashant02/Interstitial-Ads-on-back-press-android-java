# Express Coffee Machine ☕️

A simple REST API built with Express.js for managing coffees. You can add, view, update, and delete coffee items — just like operating a digital coffee machine! 🚀

---

## Features

* Add new coffees (`POST /coffees`)
* Get all coffees (`GET /coffees`)
* Get a coffee by ID (`GET /coffees/:id`)
* Update a coffee by ID (`PUT /coffees/:id`)
* Delete a coffee by ID (`DELETE /coffees/:id`)

---

## Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/express-coffee-machine.git
cd express-coffee-machine
```

### 2. Install Dependencies

```bash
npm install
```

### 3. Set Environment Variables (Optional)

* Create a `.env` file in the root directory if you want to set a custom port:

```
PORT=5000
```

### 4. Run the Server

```bash
npm start
```

* By default, server runs on [http://localhost:3000](http://localhost:3000)

---

## API Endpoints

### Add a new coffee

**POST** `/coffees`

**Body:**

```json
{
  "name": "Espresso",
  "price": 99
}
```

**Response:**

```json
{
  "id": 1,
  "name": "Espresso",
  "price": 99
}
```

---

### Get all coffees

**GET** `/coffees`

**Response:**

```json
[
  {
    "id": 1,
    "name": "Espresso",
    "price": 99
  },
  {
    "id": 2,
    "name": "Latte",
    "price": 120
  }
]
```

---

### Get a coffee by ID

**GET** `/coffees/:id`

**Response:**

```json
{
  "id": 1,
  "name": "Espresso",
  "price": 99
}
```

---

### Update a coffee by ID

**PUT** `/coffees/:id`

**Body:**

```json
{
  "name": "Americano",
  "price": 110
}
```

**Response:**

```json
{
  "id": 1,
  "name": "Americano",
  "price": 110
}
```

---

### Delete a coffee by ID

**DELETE** `/coffees/:id`

**Response:**

* `204 No Content` (with message: "deleted")

---

## Project Structure

```
express-coffee-machine/
├── node_modules/
├── .env (optional)
├── package.json
├── index.js
└── README.md
```

---

## License

[MIT](LICENSE)

---

## Contributing

Pull requests are welcome! For major changes, please open an issue first to discuss what you would like to change.

---

## Author

Made with ❤️ by Prashant
