# A11yAtlas

## Installation and running

A11yAtlas requires Node.js, npm, Git, and MongoDB. MongoDB must be installed and running before starting the application.

### 1. Clone the repository

```bash
git clone https://github.com/SiimSil/A11yAtlas.git
cd A11yAtlas
```

### 2. Install Pa11y Webservice

A11yAtlas uses Pa11y Webservice for accessibility testing data. The following command clones Pa11y Webservice into the project directory:

```bash
npm run setup:webservice
```

### 3. Install dependencies

Install the dependencies for the root project, backend, frontend, and Pa11y Webservice:

```bash
npm run install:all
```

### 4. Configure environment variables

Copy the example environment file:

```bash
cp .env.example .env
```
Then edit .env if needed. Make sure MongoDB is running at the address defined by MONGODB_URL.

### 5. Run the application

Start Pa11y Webservice, the A11yAtlas backend, and the frontend together:

```bash
npm run dev
```
Open the frontend in the browser. By default:

```bash
http://localhost:5173
```

## Commit Message Format

Use conventional commits with the following prefixes:

- **`feat:`** - New features
- **`fix:`** - Bug fixes
- **`chore:`** - Maintenance tasks (dependencies, config, etc.)
- **`docs:`** - Documentation changes

### Examples:

```bash
feat: add user authentication system
fix: resolve login validation error
chore: update package dependencies
docs: add API endpoint documentation
```
