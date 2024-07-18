# IN YOU MARKET Assignment

- IN YOU MARKET Frontend Assignment
- IN YOU MARKET DB Assignment

## IN YOU MARKET Frontend Assignment

This project is developed using Next.js, MUI, and Tailwind CSS. It has been developed responsively, adapting to mobile devices. State management is handled using Context. Unit testing is performed with @testing-library/jest-dom.

The project is deployed at: [https://inyou.wangpeifeng.com/](https://inyou.wangpeifeng.com/)

**Features**

- View user list with pagination, defaulting to 10 users per page
- Add new users
- Edit users
- Delete users

All CRUD operations update the state/context and also send corresponding RESTful requests to the test API.

The test API is a simple API written in Flask that returns 10 random users. The avatars are generated using Pravatar.

Example response:

```json
{
"avatar": "https://i.pravatar.cc/300?u=wang-1",
"company": "test-8703",
"dateJoined": "2024/07/23",
"email": "wang@wangpeifeng.com",
"id": 1,
"name": "wang 1",
"phone": "9369-1177-9767",
"username": "wang30f358901",
"website": "www.test-1.com"
}
```

### How to Use the Project

#### Install Dependencies

```bash
npm install
```

#### Run the Development Server

```bash
npm run dev
```

#### Lint the Project

```bash
npm run lint
```

This command runs ESLint to analyze the code for potential errors and enforce coding standards.

#### Format the Code

```bash
npm run format
```

This command formats the code using Prettier according to the `.prettierrc` configuration.

#### Run Unit Tests

```bash
npm run test
```

### Project Overview

#### Project Structure

```plaintext
app
├── components
│   ├── User
│   │   ├── UserDelete.test.tsx
│   │   ├── UserDelete.tsx
│   │   ├── UserDetail.test.tsx
│   │   ├── UserDetail.tsx
│   │   ├── UserList.test.tsx
│   │   ├── UserList.tsx
│   ├── Footer.tsx
│   ├── Header.tsx
├── constants
│   ├── constants.ts
├── context
│   ├── UserContext.tsx
├── handlers
│   ├── userListHandlers.ts
├── hooks
│   ├── useColumns.ts
│   ├── useUser.ts
│   ├── useUserActions.ts
├── types
│   ├── colConfig.ts
│   ├── user.ts
├── globals.css
├── layout.tsx
├── page.tsx
README.md
```

**Directory and Code Explanation**

- **components**: Contains React components used in the project.
- **constants**: Contains constant values used throughout the project.
- **context**: Contains context providers for state management.
- **handlers**: Contains handler functions for various operations.
- **hooks**: Contains custom hooks used in the project.
- **types**: Contains TypeScript type definitions.
