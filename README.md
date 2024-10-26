<h3 align="center">Frontend Developer Interview Questions (Ena Ema Technology Limited)</h3>

---

### Question 1: Merge Product Quantities
**Problem Statement:**  
You are developing a feature for an e-commerce application that tracks product transactions. Write a JavaScript function that merges an array of product transactions by `productId`, summing the `quantity`, `returnedQuantity`, and `totalQuantity` for each unique `productId`.

#### Sample Data
```javascript
const productData = [
  { productId: 29, quantity: 0, returnedQuantity: 3, totalQuantity: 5 },
  { productId: 30, quantity: 0, returnedQuantity: 3, totalQuantity: 5 },
  { productId: 29, quantity: 0, returnedQuantity: 1, totalQuantity: 1 },
  { productId: 30, quantity: 0, returnedQuantity: 1, totalQuantity: 1 }
];
```

#### Expected Output
```javascript
[
  { productId: 29, quantity: 0, returnedQuantity: 4, totalQuantity: 6 },
  { productId: 30, quantity: 0, returnedQuantity: 4, totalQuantity: 6 }
]
```

#### Function Signature
```javascript
function mergeProducts(products) {
  // Your code here
}
```

**Follow-Up:**  
How would you modify the function if both `productId` and `purchaseId` were used for uniqueness?

---

### Question 2: Library Book Search

**Problem Statement:**  
You are developing a library management system where users can search for books. Write a function called `searchBooks` that accepts an array of book objects and a search term. The function should return an array of book titles that include the search term (case-insensitive).

**Example Input:**
```javascript
const books = [
  { title: 'The Great Gatsby', author: 'F. Scott Fitzgerald' },
  { title: 'To Kill a Mockingbird', author: 'Harper Lee' },
  { title: '1984', author: 'George Orwell' },
  { title: 'The Catcher in the Rye', author: 'J.D. Salinger' }
];
const searchTerm = 'the';
```

**Expected Output:**
```javascript
['The Great Gatsby', 'The Catcher in the Rye']
```



---

### Question 3: User Registration Validation
**Problem Statement:**  
You are developing a user registration form for a web application. Write a function called `validateUserInput` that accepts an object with user information (name, email, and password) and validates it. The function should return an object indicating whether the input is valid and any relevant error messages. The validation rules are as follows:
- Name should be at least 3 characters long.
- Email must contain an '@' symbol and a domain (e.g., '.com').
- Password should be at least 6 characters long.

#### Example Input
```javascript
const userInput = {
  name: 'Jo',
  email: 'jo@example',
  password: '123'
};
```

#### Expected Output
```javascript
{
  isValid: false,
  errors: {
    name: 'Name must be at least 3 characters long.',
    email: 'Email must be a valid email address.',
    password: 'Password must be at least 6 characters long.'
  }
}
```
