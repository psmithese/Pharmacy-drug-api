# Pharmacy Drug API

A comprehensive RESTful API built with Express.js for managing pharmaceutical data, allowing users to filter, search, and analyze drug information by various parameters.

## 📋 Overview

This API provides multiple endpoints to query a database of pharmaceutical drugs, filter by categories, check prescription requirements, monitor stock levels, and analyze drug distribution by manufacturer.

## 🚀 Getting Started

### Prerequisites

- Node.js (v14 or higher)
- npm (v6 or higher)

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/psmithese/pharmacy-drug-api.git
   cd pharmacy-drug-api
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Start the server:
   ```bash
   npm start
   ```

The server will run on port 8000 by default or use the port specified in your environment variables.

## 🛠️ API Endpoints

#### 1. Get all antibiotics
```
GET /drugs/antibiotics
```
Returns all drugs in the "Antibiotic" category.

#### 2. Get drug names in lowercase
```
GET /drugs/lowercase-names
```
Returns an array containing all drug names converted to lowercase.

#### 3. Get drugs by category
```
GET /drugs/by-category
```
Returns all drugs that belong to the specified category.

#### 4. Get drug and manufacturer information
```
GET /drugs/names-manufacturer
```
Returns a list of all drugs with their manufacturers and logs this information to the console.

#### 5. Get prescription-only drugs
```
GET /drugs/prescription
```
Returns all drugs that require a prescription.

#### 6. Get formatted drug information
```
GET /drugs/formatted
```
Returns drugs in the format: "Drug: [name] - [dosageMg]mg"

#### 7. Get drugs with low stock
```
GET /drugs/low-stock
```
Returns all drugs with stock levels below the specified limit (defaults to 50 if not provided).

#### 8. Get over-the-counter drugs
```
GET /drugs/non-prescription
```
Returns all drugs that do not require a prescription.

#### 9. Count drugs by manufacturer
```
GET /drugs/manufacturer-count
```
Returns the count of drugs from a specific manufacturer along with their details.

#### 10. Count drugs by category
```
GET /drugs/count-analgesics
```
Returns the count of drugs in a specific category (defaults to "Analgesic" if not specified).

## 📝 Sample Data

The API includes a dataset of 20 pharmaceutical drugs with the following properties:
- id
- name
- category
- dosageMg
- isPrescriptionOnly
- stock
- manufacturer

## 🔧 Technology Stack

- Node.js
- Express.js
- JavaScript

## 📄 License

This project is licensed under the MIT License - see the LICENSE file for details.

## 👨‍💻 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the project
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request
