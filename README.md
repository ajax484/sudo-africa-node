
# 📖 SudoAfrica SDK

Easily integrate with Sudo Africa services, providing a comprehensive API for managing customers.

## 📦 Installation

```bash
npm install sudo-africa-node
```

## 🚀 Getting Started

Firstly, you need to instantiate the `SudoAfrica` class:

```javascript
const SudoAfrica = require('sudoafrica-sdk');
const sudoInstance = new SudoAfrica('YOUR_API_KEY', 'YOUR_BASE_URL');
```

## 📝 API

### 🔷 createCustomer(data)

Create a new customer.

**Arguments**:

- `data`: Object - Customer details.

**Returns**:

- Promise<Object> - The created customer data.

### 🔷 getCustomers(page, limit)

Retrieve a list of customers.

**Arguments**:

- `page`: Number (default: 0) - Page number.
- `limit`: Number (default: 100) - Number of results per page.

**Returns**:

- Promise<Array> - List of customers.

### 🔷 getCustomerById(customerId)

Retrieve a specific customer.

**Arguments**:

- `customerId`: String - The customer's ID.

**Returns**:

- Promise<Object> - The customer's data.

### 🔷 updateCustomer(customerId, customerData)

Update an existing customer.

**Arguments**:

- `customerId`: String - The customer's ID.
- `customerData`: Object - New data for the customer.

**Returns**:

- Promise<Object> - The updated customer data.

### 🔷 updateCustomerDocumentUrl(customerId, fileName, fileType)

Update a customer's document URL.

**Arguments**:

- `customerId`: String - The customer's ID.
- `fileName`: String - Name of the file.
- `fileType`: String - Type of the file (e.g., 'image').

**Returns**:

- Promise<Object> - Response data.

## 🔗 Links

- [GitHub Repository](https://github.com/ibroraheem/sudo-africa-node)
- [Official Documentation](https://docs.sudo.africa)
- [Issues & Feature Requests](https://github.com/ibroraheem/sudo-africa-node/issues)
