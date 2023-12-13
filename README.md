# Official OpenCore Group Website

This is the official website for OpenCore Group. This repository will serve the following purposes:

1. Hold all the source code related to this project
2. Contain relevant documentation such as the repository structure, getting started, etc.
3. Contain best practices to update and make changes

### 🚀 Getting Started

Follow these steps to get started with this project:

1. **Fork the Repository**: Click on the 'Fork' button at the top right corner of this page. This will create a copy of this repository in your GitHub account.

2. **Clone the Repository**: Now, clone the forked repository to your machine. Go to your GitHub account, open the forked repository, click on the 'Code' button and then click the 'copy to clipboard' icon to get the clone command. Open a terminal and run the following git command:

   ```bash
   git clone "COPIED_URL_IN_CLIPBOARD"
   ```

3. **Navigate to the Project Directory**: Use the following command to navigate to the project directory:

   ```bash
   cd OpenCore-Group-Official-Website
   ```

4. **Install Dependencies**: Now, run the following command to install all the project dependencies:

   ```bash
   npm install
   ```

5. **Start the Project**: Finally, you can start the project by running:
   ```bash
   npm run dev
   ```
   The dev server will start on `http://localhost:3000`.

### 📁 Repository Structure

A template of the repository structure being used in this project can be seen below:

```
├── public
├── src
│   ├── app
│   │   ├── (home)
│   │   │   ├── _components
│   │   │   │   ├── Hero.tsx
│   │   │   │   └── ...
│   │   │   ├── layout.tsx
│   │   │   └── page.tsx
│   │   ├── about
│   │   │   └── ...
│   │   ├── work
│   │   │   └── ...
│   │   └── contact
│   │       └── ...
│   ├── components
│   │   └── ui
│   │       ├── Button.tsx
│   │       ├── Alert.tsx
│   │       └── ...
│   └── lib
│       ├── hooks
│       │   ├── useHook.tsx
│       │   └── ...
│       ├── contexts
│       │   ├── ModalContext.tsx
│       │   └── ...
│       ├── types
│       │   ├── Employee.ts
│       │   └── ...
│       └── helpers
│           ├── addInts.ts
│           └── ...
├── next.config.js
├── package.json
├── package-lock.json
├── postcss.config.js
├── tailwind.config.ts
└── tsconfig.json
```

Some notes about the `src` folder:

#### app

    The app folder is used to hold all routes/pages. (parentheses) are used to group routes without creating a new route. This may be useful if you want to create a unique layout for a group of routes that differ from the rest.

#### components

    The components folder will hold all the reusable UI components for this project. This includes but is not limited to things like buttons, alerts, inputs, modals, etc.

#### lib

    The lib folder is used to hold all utilities that are not direct UI or route-specific components/types. This will be used to house global types, helper functions, hooks, contexts, and other related items.

### 🔤 Naming Conventions

Below are the naming conventions that are used throughout this project:

1. Files: Use PascalCase for filenames (with the exception of `layout.tsx` and `page.tsx` being camelCase). Example: `MyComponent.tsx, MyInterface.ts, MyEnum.ts`.

2. Components: Use PascalCase for React components. Example: `const MyComponent = () => {};`.

3. Interfaces: Use PascalCase and prefix with "I". Example: `interface IMyInterface {}`.

4. Enums: Use PascalCase. Example: `enum MyEnum {}`.

5. Functions: Use camelCase. Example: `const myFunction = () => {};`.

6. Variables: Use camelCase. Example: `const myVariable = 'value';`.

7. Folders: Use kebab-case. Example: `my-folder`.
