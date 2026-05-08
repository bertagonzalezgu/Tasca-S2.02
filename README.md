# Sprint 2 - TypeScript Basics (Solved)

This repository contains my solutions for the IT Academy Sprint 2 practical exercises. The goal of this project was to master fundamental TypeScript concepts, ranging from basic static typing to advanced type transformations.

## Technologies Used

- **TypeScript**: Main language used for static typing and type safety.
- **Vitest**: Testing framework used to validate the solutions.
- **Husky**: Automated Git hooks to ensure code quality before every commit.

## Installation & Usage

1. **Clone this repository:**
   ```bash
   git clone https://github.com/bertagonzalezgu/Tasca-S2.02.git
   cd it-sprint2-basics-ts

2. **Install dependencies:**
    ```bash
    npm install
Run the tests to verify solutions:

    ```bash
    npm test          # Runs all tests with Vitest
    npm run test:types # Validates that there are no TypeScript compilation errors

## Project Content
The exercises are organized into two main test files:

1. **Basics Refactor** (basics-refactor.test.ts)

    18 challenges covering core TypeScript features:
    
    Object & Function Typing: Using optional properties (?) and typed parameters.
    
    Interfaces & Inheritance: Applying the DRY (Don't Repeat Yourself) principle using extends.
    
    Unions & Intersections: Restricting values with unions (|) and merging types with intersections (&).
    
    Async Logic: Typing Promises and async/await functions.
    
    Basic Utility Types: Practical usage of Pick and Omit.

2. **Transformation Types** (transformation-types.test.ts)
    13 challenges focusing on advanced type manipulation:
    
    Type Inference: Leveraging typeof and as const for literal types.
    
    Advanced Utility Types: Using ReturnType, Parameters, Awaited, and Record.
    
    Indexed Access Types: Extracting types from object keys (T["key"]) or array indexes (T[number]).
    
    Discriminated Unions: Filtering complex unions using Extract and Exclude.
    
    Terminology: Deep dive into the differences between Union, Discriminated Union, and Enum.

## Key Takeaways
Through these exercises, I have mastered essential TypeScript patterns:

Discriminated Unions: Using a shared property (like type or kind) to allow TypeScript to perform "Type Narrowing" inside logic blocks.

Exclusion vs. Extraction: Knowing when to subtract types from a union (Exclude) or specifically select them (Extract).

Return Type Safety: Ensuring that functions, especially asynchronous ones, strictly adhere to their promised data structures.

## Code Quality & Git Hooks
This project uses Husky to automate code validation. Whenever a git commit is attempted, Husky automatically triggers:

npm run test

npm run test:types

If any validation fails, the commit is blocked. This ensures that the repository remains clean and free of type-related bugs or broken tests.

## License

GPL-3.0
