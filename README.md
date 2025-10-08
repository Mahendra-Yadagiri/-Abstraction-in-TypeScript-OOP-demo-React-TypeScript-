# -Abstraction-in-TypeScript-OOP-demo-React-TypeScript-
Single-page React + TypeScript demo demonstrating abstraction and OOP using an abstract Animal class with Lion, Tiger, and Cat children. Shows runtime console behavior, componentized UI, and step-by-step comments for learners. Great for exploring extensibility, clean TypeScript architecture, and testable design. MIT. Deployable to Netlify. README.
# Animal Abstraction — TypeScript + React

A small educational project demonstrating **abstraction** and OOP patterns in TypeScript inside a React single-page app.


## Overview
This project uses a parent `Animal` **abstract class** that defines shared behaviour (e.g., `eat()`, `sleep()`), and child classes (`Lion`, `Tiger`, `Cat`) that implement specific details. The app creates instances and logs lifecycle/runtime behaviour to the browser console so you can observe abstraction in action.

## Tech stack
- React (TypeScript)
- Vite or Create React App (your choice)
- CSS for layout
- Deployable to Netlify

## Features
- Pure TypeScript OOP: abstract classes and interfaces
- Componentized React UI
- Console logs that show runtime behavior for each animal
- Clear comments and readable code for learning

## Example (TypeScript)
**Animal.ts**
```ts
export abstract class Animal {
  constructor(public name: string) {}

  abstract sleep(): void;
  abstract eat(): void;

  describe(): string {
    return `${this.name} (type: ${this.constructor.name})`;
  }
}
