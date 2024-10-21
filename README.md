# README

## Project Overview

** Sykooo is an e-commerce platform built using MedusaJS deployed on Railway App. It leverages Next.js Storefront for a seamless user experience and Tailwind CSS for efficient styling. Razorpay is integrated for secure payment processing, and Google Analytics provides valuable insights into user behavior. **

> Key Features

- MedusaJS Backend: A robust and scalable e-commerce platform.
- Next.js Storefront: Provides a modern and performant frontend.
- Tailwind CSS: Simplifies styling with utility-first classes.
- Razorpay: Enables secure and efficient payment processing.
- Google Analytics: Offers insights into user behavior and website performance.

> Getting Started
> Clone the Repository:

```
{
git clone https://github.com/your-username/sykooo.git
# Use code with caution.
}


# Install Dependencies:
# Bash
cd sykooo
npm install
# Use code with caution.


# Set Up Environment Variables: Create a .env file in the project root and add the following variables:
MEDUSA_URL: Your MedusaJS backend URL
MEDUSA_ADMIN_SECRET_KEY: Your MedusaJS admin secret key
RAZORPAY_KEY_ID: Your Razorpay key ID
RAZORPAY_KEY_SECRET: Your Razorpay key secret
GOOGLE_ANALYTICS_ID: Your Google Analytics tracking ID
# Running the Project
# Start the Development Server:
Bash
npm run dev
# Use code with caution.
```

## The project will be accessible at http://localhost:3000.

Deployment
Railway App:

### Create a new Railway project.

Connect your GitHub repository.
Set up environment variables as described in the "Setting Up Environment Variables" section.
Deploy the project.

### Contributing

Contributions are welcome! Please follow these guidelines:
Fork the repository.
Create a new branch for your feature or bug fix.  
Make your changes.  
Commit your changes with descriptive commit messages.
Push your changes to your fork.
Create a pull request to the main branch.  
License
This project is licensed under the MIT License.

Sources and related content

## About this boilerplate

This boilerplate is a monorepo consisting of snapshot of newly released medusajs 2.0 (release candidate) backend and storefront app created with `npx create-medusa-app@rc` October 2024. Modified to be plug n' play deployable on [railway.app](https://railway.app?referralCode=-Yg50p)!

Updated: to `version 2.0.0-rc`

# /backend

### local setup

Video instructions: https://youtu.be/PPxenu7IjGM

- Install dependencies `npm i`
- Rename `.env.template` -> `.env`
- To connect to your online database, from local; copy the `DATABASE_URL` value that have been auto generated on railway, and add to your `.env`

### requirements

- **postgres database** (will be automatically generated if using railway template)
- **redis** (will be automatically generated if using railway template)

### commands

`cd backend/`
`npm run dev` will start backend (and admin dasboard frontend on `localhost:9000/app`) - in development mode

# /storefront

### local setup

Video instructions: https://youtu.be/PPxenu7IjGM

intall dependencies `npm i`
Rename `.env.local.template` -> `.env.local`

### requirements

- running backend on port 9000 - needed to fetch products data and more, to build nextjs pages.

### commands

`cd storefront/`
`npm run dev` will run on uncompiled code, and hot-reload as files saved with changes

## Useful resources

- How to setup credit card payment with Stripe payment module: https://youtu.be/dcSOpIzc1Og
- https://funkyton.com/medusajs-2-0-is-finally-here/#succuessfully-deployed-whats-next
