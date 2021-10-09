# MySQL +NextJs



## Deploy your own

Once you have access to [the environment variables you'll need](#step-5-set-up-environment-variables), deploy the example using [Vercel](https://vercel.com?utm_source=github&utm_medium=readme&utm_campaign=next-example):


## How to use

```bash
npx create-next-app --example with-mysql next-mysql-app
# or
yarn create next-app --example with-mysql next-mysql-app
```

## Configuration

### Step 1. Set up a MySQL database

Set up a MySQL server either locally or any cloud provider.

### Step 2. Set up environment variables

Copy the `env.local.example` file in this directory to `.env.local` (which will be ignored by Git):

```bash
cp .env.local.example .env.local
```

Set each variable on `.env.local`:

- `MYSQL_HOST` - Your MySQL host URL.
- `MYSQL_DATABASE` - The name of the MySQL database you want to use.
- `MYSQL_USERNAME` - The name of the MySQL user with access to database.
- `MYSQL_PASSWORD` - The passowrd of the MySQL user.

### Step 3. Run migration script

You'll need to run a migration to create the necessary table for the example.

```bash
npm run migrate
# or
yarn migrate
```

### Step 4. Run Next.js in development mode

```bash
npm install
npm run dev
# or
yarn install
yarn dev
```


#### Deploy Your Local Project

To deploy your local project to Vercel, push it to GitHub/GitLab/Bitbucket and [import to Vercel](https://vercel.com/new?utm_source=github&utm_medium=readme&utm_campaign=next-example).

**Important**: When you import your project on Vercel, make sure to click on **Environment Variables** and set them to match your `.env.local` file.

