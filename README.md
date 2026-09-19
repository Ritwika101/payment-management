# Payment Management System

A backend application for managing trip assignments, Proof of Delivery (POD) verification, and driver payments through role-based workflows.

## Features

- JWT-based authentication and role-based authorization
- Admin, Driver, and Payment Executive roles
- Trip creation and driver assignment
- Driver trip start/completion workflows
- Proof of Delivery (POD) upload and verification
- Rate-card based payment calculation
- Automatic incentive and penalty calculation
- Asynchronous payment-request generation using Redis Bull
- Driver ledger and payment tracking
- Paginated APIs for users, payments, and ledgers

## Payment Workflow

`Trip Created → Driver Assigned → Trip Completed → POD Submitted → POD Approved → Payment Request Generated → Payment Processed`

Payment requests are generated asynchronously after POD approval. The payable amount is calculated using the trip's rate card, actual distance travelled, incentives, and penalties.

## Tech Stack

- Node.js
- Express.js
- MongoDB & Mongoose
- Redis
- Bull
- JWT
- bcrypt
- Multer
- Socket.IO
- EJS

## Core Modules

- Users & Authentication
- Trips
- Rate Cards
- POD Verification
- Payment Requests
- Driver Ledger
- Background Payment Processing


## Author

**Ritwika Pal**
