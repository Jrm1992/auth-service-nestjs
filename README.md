# NestJS Authentication Project

<p align="center">
  <a href="http://nestjs.com/" target="blank"><img src="https://nestjs.com/img/logo-small.svg" width="200" alt="Nest Logo" /></a>
</p>

[circleci-image]: https://img.shields.io/circleci/build/github/nestjs/nest/master?token=abc123def456
[circleci-url]: https://circleci.com/gh/nestjs/nest

  <p align="center">A progressive <a href="http://nodejs.org" target="_blank">Node.js</a> framework for building efficient and scalable server-side applications.</p>
    <p align="center">
<a href="https://www.npmjs.com/~nestjscore" target="_blank"><img src="https://img.shields.io/npm/v/@nestjs/core.svg" alt="NPM Version" /></a>
<a href="https://www.npmjs.com/~nestjscore" target="_blank"><img src="https://img.shields.io/npm/l/@nestjs/core.svg" alt="Package License" /></a>
<a href="https://www.npmjs.com/~nestjscore" target="_blank"><img src="https://img.shields.io/npm/dm/@nestjs/common.svg" alt="NPM Downloads" /></a>
<a href="https://circleci.com/gh/nestjs/nest" target="_blank"><img src="https://img.shields.io/circleci/build/github/nestjs/nest/master" alt="CircleCI" /></a>
<a href="https://coveralls.io/github/nestjs/nest?branch=master" target="_blank"><img src="https://coveralls.io/repos/github/nestjs/nest/badge.svg?branch=master#9" alt="Coverage" /></a>
<a href="https://discord.gg/G7Qnnhy" target="_blank"><img src="https://img.shields.io/badge/discord-online-brightgreen.svg" alt="Discord"/></a>
<a href="https://opencollective.com/nest#backer" target="_blank"><img src="https://opencollective.com/nest/backers/badge.svg" alt="Backers on Open Collective" /></a>
<a href="https://opencollective.com/nest#sponsor" target="_blank"><img src="https://opencollective.com/nest/sponsors/badge.svg" alt="Sponsors on Open Collective" /></a>
  <a href="https://paypal.me/kamilmysliwiec" target="_blank"><img src="https://img.shields.io/badge/Donate-PayPal-ff3f59.svg"/></a>
    <a href="https://opencollective.com/nest#sponsor"  target="_blank"><img src="https://img.shields.io/badge/Support%20us-Open%20Collective-41B883.svg" alt="Support us"></a>
  <a href="https://twitter.com/nestframework" target="_blank"><img src="https://img.shields.io/twitter/follow/nestframework.svg?style=social&label=Follow"></a>
</p>
  <!--[![Backers on Open Collective](https://opencollective.com/nest/backers/badge.svg)](https://opencollective.com/nest#backer)
  [![Sponsors on Open Collective](https://opencollective.com/nest/sponsors/badge.svg)](https://opencollective.com/nest#sponsor)-->


This is a simple and straightforward NestJS project for implementing user authentication using Prisma ORM, JWT (JSON Web Tokens), Bcrypt for password hashing, Class-Validator for input validation, Class-Transformer for data transformation, and Passport for authentication.

## Getting Started

Follow these steps to set up and run this project on your local machine.

### Prerequisites

Before you begin, ensure you have Node.js and npm (Node Package Manager) installed on your machine. You'll also need a PostgreSQL database to store user information.

### Installation

1. Clone this repository to your local machine:

   ```bash
   git clone https://github.com/your-username/nestjs-authentication-project.git
   ```

2. Navigate to the project directory:

   ```bash
   cd nestjs-authentication-project
   ```

3. Install the project dependencies:

   ```bash
   npm install
   ```

### Configuration

1. Create a `.env` file in the project's root directory and set the following environment variables:

   ```dotenv
   DATABASE_URL=postgresql://username:password@localhost:5432/database
   JWT_SECRET=mysecretkey
   ```

   Replace `username`, `password`, `localhost`, `5432`, `database`, and `mysecretkey` with your PostgreSQL database credentials and a secret key for JWT.

### Database Migration

1. Run the Prisma migration to create the necessary database tables:

   ```bash
   npx prisma migrate dev
   ```

2. Seed the database with initial data (optional):

   ```bash
   npx prisma db seed
   ```

### Start the Application

1. Start the NestJS application:

   ```bash
   npm run start
   ```

The application should now be running on `http://localhost:3000`.


## Features

- User registration and authentication
- Password hashing with Bcrypt
- JSON Web Token (JWT) authentication
- Input validation using Class-Validator
- Data transformation with Class-Transformer
- PostgreSQL database storage with Prisma ORM
- Passport for authentication strategies (if needed)

## Contributors

- [Your Name](https://github.com/your-username)

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details.

## Acknowledgments

- [NestJS](https://nestjs.com/)
- [Prisma](https://www.prisma.io/)
- [JWT](https://jwt.io/)
- [Bcrypt](https://www.npmjs.com/package/bcrypt)
- [Class-Validator](https://github.com/typestack/class-validator)
- [Class-Transformer](https://github.com/typestack/class-transformer)
- [Passport](http://www.passportjs.org/)

Feel free to modify and enhance this project according to your needs. Happy coding!
