# React Product Store

A responsive product listing web application built with **React.js** that fetches product data from the **Fake Store API** and displays it in a clean product-card layout.

## 🚀 Features

* Fetches products from Fake Store API
* Displays product images
* Displays product titles and prices
* Shows product ratings and review counts
* Responsive product grid
* Reusable React components
* Uses React Hooks
* Loading data using `useEffect`
* Product state management using `useState`

## 🛠️ Technologies Used

* React.js
* JavaScript (ES6+)
* HTML5
* CSS3
* Fetch API
* Fake Store API
* Vite

## 📂 Project Structure

```text
react-product-store/
│
├── public/
│
├── src/
│   ├── App.jsx
│   ├── App.css
│   ├── main.jsx
│   └── index.css
│
├── .gitignore
├── package.json
├── package-lock.json
└── README.md
```

## ⚙️ Installation

### 1. Clone the repository

```bash
git clone https://github.com/YOUR-USERNAME/react-product-store.git
```

### 2. Open the project

```bash
cd react-product-store
```

### 3. Install dependencies

```bash
npm install
```

### 4. Start the development server

```bash
npm run dev
```

The application will run on the local development server provided by Vite.

## 🔗 API Used

This project uses the Fake Store API to retrieve product information.

**API Endpoint:**

```text
https://fakestoreapi.com/products
```

The API provides information such as:

* Product ID
* Product title
* Price
* Image
* Category
* Rating
* Review count

## 💡 React Concepts Practiced

### useState

Used to store the products received from the API.

```javascript
const [products, setProducts] = useState([]);
```

### useEffect

Used to fetch the products when the component loads.

```javascript
useEffect(() => {
  fetch("https://fakestoreapi.com/products")
    .then((res) => res.json())
    .then((data) => setProducts(data));
}, []);
```

### map()

Used to dynamically render each product.

```javascript
products.map((product) => (
  <div key={product.id}>
    {product.title}
  </div>
))
```

## 🔮 Future Improvements

* Add product search
* Add category filtering
* Add sorting by price
* Add product details page
* Add shopping cart
* Add quantity management
* Add React Router
* Add loading spinner
* Add error handling
* Add dark mode

## 🎯 Learning Goal

This project was created to practice **React.js fundamentals**, especially API fetching, state management, `useEffect`, rendering lists with `map()`, and creating responsive UI layouts.

## 👩‍💻 Author

**Lakshmi Thalluru**

B.Tech CSE Student | Aspiring Full Stack Developer

## ⭐ Support

If you find this project useful, consider giving the repository a ⭐ on GitHub.
