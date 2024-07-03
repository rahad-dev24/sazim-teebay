//clone this repo using
`git clone --recursive https://github.com/rahad-dev24/sazim-teebay.git`

//Installation Instructions

***First run `docker compose up` to start the frontend and database server. 

( Assming you have docker installed this might take some time. This step is taken to make the frontend and the database as production ready as possible. If this is taking too long foy you, just cd to the frontend folder and run `npm i && npm run dev` or `npm i && npm run build && npm run start`. As for the database change the .env file in backend folder and give necessary URL. )

***Then cd to the backend folder and run `npm install` to install the packages after that run `npm run start` to start the backend server and redis server. 

(Assuming you have node, npm and redis installed)


frontend, backend and database are running on port 3000, 4000 and 5432 respectively.


-----------------------------------------------------------------
// Short Manual

Go to localhost:3000 or localhost:3000/login to login as a user.

Create an account by going to localhost:3000/signup.

Create a product by going to localhost:3000/dashboard/add-product and fill in the form.

After creating a product you and other users can see it in the landing page and users can buy and rent it. You can also see it in the dashboard.

Edit or delete product from the dashboard.

Bought, Sold, Borrowed and Lented products can be seen in the dashboard.


-----------------------------------------------------------------
// Technologiees

Frontend technonologies used: Next.js, Tailwindcss, shadcn/ui, Zod, React-hook-form, Apollo-client, Nodemon, Docker, Docker Compose.


Backend technologies used: Node, Express, Prisma, Postgres, Redis.


-----------------------------------------------------------------
// Some Edge Cases

There are many edge cases in the project for example the borroewer and lender can not be the same user. If the rental period is exceeds the time linit and the product is not returned, the borrower would be charged per day on their account.

There should be return policy for products.

If the product is damaged, it should be returned within 7 days.

If Borrowed product is damaged or stolen, the borrower should be charged for the full price of the product.







