## Stack
- Next.js 15
- App Router
- Server Actions
- Drizzle ORM
- Turso Database
- Todo CRUD
- TypeScript
- Tailwind CSS

## Local Development
1. Clone this repository
2. Install dependencies:
   ```bash
   npm install
   ```
3. Set up your environment variables:
   ```bash
   cp .env.example .env
   ```
   Fill in your Turso database credentials:
   ```
   TURSO_DATABASE_URL=your_turso_database_url
   TURSO_AUTH_TOKEN=your_turso_auth_token
   ```
4. Set up your database:
   ```bash
   npm run db:generate
   npm run db:push
   ```
5. Start the development server:
   ```bash
   npm run dev
   ```
   
## Database Management
This project uses Drizzle ORM for database operations. Here are the available commands:
- `npm run db:generate` - Generate migration files from schema changes
- `npm run db:push` - Push schema changes directly to the database (use with caution)
- `npm run db:migrate` - Run migrations against the database
- `npm run db:studio` - Open the Drizzle Studio for database management