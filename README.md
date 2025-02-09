Recipy library
======================

Free quickstart recipe libary app using [Next.js](https://nextjs.org/), [Prisma](https://www.prisma.io/) and [Aiven](https://aiven.io). Recipe data is from [kaggle](https://www.kaggle.com/datasets/thedevastator/better-recipes-for-a-better-life).

About the app
========

The application is a recipe library where you can browse and inspect recipes. Additionally, you can like recipes that seem interesting and filter list to show only liked ones. Furthermore, you can see interesting statistics from all of the recipes and those that are liked.

PostgreSQL® is used as the data storage for storing all recipes and whether they are liked or not. Aiven for Caching is optional, but when configured statistics are cached to offer faster response time. The database response times are shown in the app to demonstrate the difference. You can get free services with Aiven for PostgreSQL and Aiven for Caching by [signing up](https://console.aiven.io/signup).

Getting started
============

The app requires a PostgreSQL database. Configuring Aiven for Caching is optional, but highly recommended to demonstrate all features of the application and the benefits of having Caching as part of your application.

Get free Aiven for PostgreSQL and Aiven for Caching from [Aiven](https://console.aiven.io/singup).

## Development setup

- Install Node version 18
- Copy [.env.template](.env.template) as .env and set DATABASE_URL and REDIS_URI
- Install the packages: `npm ci`
- Setup the database by running: `npm run reset-db`
- Start the development server: `npm run dev`
- Go to http://localhost:3000 and head to browse the recipes

Congratulations you can now start developing. The page reloads automatically as you make changes.

## Useful commands for development

- Reset the database: `npm run reset-db`
- Run the development server: `npm run dev`
- Run eslint: `npm run eslint`
- Run prettier format: `npm run format`

Licenses
============
Project is originated from [nextjs-netlify](https://github.com/Aiven-Labs/nextjs-netlify).

nextjs-netlify is licensed under the Apache license, version 2.0. Full license text is available in the [LICENSE](LICENSE) file.
Please note that the project explicitly does not require a CLA (Contributor
License Agreement) from its contributors.

PostgreSQL is a trademark or registered trademark of the PostgreSQL Community Association of Canada, and used with their permission.
*Redis is a registered trademark of Redis Ltd. Any rights therein are reserved to Redis Ltd. 
Any use by Aiven is for referential purposes only and does not indicate any sponsorship, endorsement or affiliation between Redis and Aiven.  All product and service names used in this website are for identification purposes only and do not imply endorsement.
