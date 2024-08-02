<h1 align="center">Node Express Typescript Prisma Postgres Boilerplate</h1>

<p align="center">🦄 Starter template for your Express Prisma Postgres API</p>

![npm i cart](images/cover.png)


## 🍔 Stack Specs

- Node.js
- Express
- TypeScript
- Prisma
- Postgres

## 🧬 Development

- Clone the repository

```
git clone https://github.com/mcnaveen/node-express-typescript-prisma-postgres-boilerplate api-boilerplate
```
- Cd into the project directory
```
cd api-boilerplate
```

> I'm using `pnpm` as a package manager. You can also use package manager of your choice.


- Install dependencies

```
pnpm install
```

- Create a Database in Postgres (or) You can use GUI to create a database

```
postgres=# CREATE DATABASE express;
```

- Copy the `.env.sample` file as `.env`

```
cp .env.sample .env
```

- Edit the Postgres Details in the `.env` file

```
DATABASE_URL="postgresql://postgres:password@dev@localhost:5432/express"
```

- Push the Prisma Schema into Database

```
npx prisma migrate dev
```

- Run the development server

```
pnpm dev
```

## 🚀 Production Build

- Run the production build

```
pnpm build
```

- Start the production server

```
pnpm start
```

> Your production build is available on `dist` folder

## 🧭 Endpoints

- `POST` - For Creating New User
- `GET` - For Getting All Users
- `GET` - For Getting User By ID
- `PATCH` - For Updating User By ID
- `DELETE` - For Deleting User By ID

## 🃏 Examples

> 💡 Please install the Recommended VS Code Extensions and Check `api.rest` file for Examples

- Creating a New User

```
POST http://localhost:4000/users
Content-Type: application/json

{
  "name": "john",
  "email": "john@gmail.com"
}
```

- Getting All Users

```
GET http://localhost:4000/users
```

- Getting User By ID

```
GET http://localhost:4000/users/1
```

- Patching User By ID

```
PATCH http://localhost:4000/users/1
Content-Type: application/json

{
  "name": "newjohn",
  "email": "john@gmail.com"
}
```

- Deleting User By ID

```
DELETE http://localhost:4000/users/1
```

## ☑️ LICENSE
- MIT

---
### 💰 HELP ME WITH DEVELOPMENT COST

<a href="https://www.buymeacoffee.com/mcnaveen" target="_blank"><img src="https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png" alt="Buy Me A Coffee" style="height: 41px !important;width: 174px !important;box-shadow: 0px 3px 2px 0px rgba(190, 190, 190, 0.5) !important;-webkit-box-shadow: 0px 3px 2px 0px rgba(190, 190, 190, 0.5) !important;" ></a>
