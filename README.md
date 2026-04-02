# Real Estate Database Project

This project is a PHP web application developed using **XAMPP**. It interacts with a relational database that manages information about real estate spaces, agencies, types, and offers.

---

## Database Structure

The database consists of four tables:

| Table    | Columns                                    | Description                               |
|----------|--------------------------------------------|-------------------------------------------|
| Agency   | `id_agentie` (PK), `nume`                 | Stores agency details                     |
| Space    | `id_spatiu` (PK), `adresa`, `zona`, `suprafata`, `id_tip` | Stores information about spaces           |
| Type     | `id_tip` (PK), `denumire`, `caracteristici` | Defines types of spaces                    |
| Offer    | `id_agentie`, `id_spatiu` (PK), `vanzare`, `pret`, `moneda` | Contains offers made by agencies for spaces |

---

## Project Requirements and Queries

### 3. Space and Offer Details
- **a)** Retrieve spaces whose address has `'j'` in the third character, ordered by `zona` ascending and `suprafata` descending.  
- **b)** Retrieve offers of type **sale** with a price below 70,000 EUR, or its equivalent in the offer currency (RON/USD) based on the current exchange rate.  

### 4. Apartment Rentals and Price Comparisons
- **a)** For type **apartment**, retrieve rental offers under 250 EUR or equivalent in RON/USD.  
- **b)** Find unique pairs of agencies offering the same space for sale at different prices (considering currency exchange).  

### 5. Specific Space Queries
- **a)** Retrieve **garage** spaces in zone 2 with the largest surface area.  
- **b)** Find agencies offering spaces of the same type, price, and currency as **AgentieRoyal** for space `id_spatiu` 111.  

### 6. Price Statistics
- **a)** Find the minimum, average, and maximum price per currency and sale type for **apartments**.  
- **b)** For each zone and currency, calculate the total rental price and the number of apartment rental offers.  

---

## Technologies Used
- PHP  
- MySQL / MariaDB (via XAMPP)  
- HTML/CSS for frontend
