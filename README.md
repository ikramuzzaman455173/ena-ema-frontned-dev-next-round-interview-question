

## Frontend Developer Interview Questions (Ena Ema Technology Limited)

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

### Question 2: Inventory Management
**Problem Statement:**  
You are building an inventory management system for a small retail store. You have an array of product objects, each with a name and quantity. Write a function called `getLowStockProducts` that takes this array and a threshold quantity as parameters. The function should return an array of product names that are below the given threshold quantity.

#### Example Input
```javascript
const products = [
  { name: 'Apples', quantity: 5 },
  { name: 'Bananas', quantity: 2 },
  { name: 'Cherries', quantity: 15 },
  { name: 'Dates', quantity: 1 }
];
const threshold = 3;
```

#### Expected Output
```javascript
['Bananas', 'Dates']
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
