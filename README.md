# TypeScript & OOP Problem Solving (Assignment-1)

This repository contains solutions for **Assignment-1 (B8A1)**, covering essential TypeScript concepts including type narrowing, readonly tuples, interfaces, generics, Object-Oriented Programming (OOP) with access modifiers, and asynchronous Promises.

---

## 📂 File Structure

```text
.
├── solutions.ts
├── any-unknown-never.md
├── generics-and-promises.md
└── README.md
```

---

## 🚀 Solutions Overview

All required problem-solving tasks are implemented in [`solutions.ts`](./solutions.ts) with strict type safety, explicit parameter and return types, and zero `any` usage:

1. **`multiplyValue`**: Handles optional and default multipliers, properly accounting for numeric `0`.
2. **`processInput`**: Uses `typeof` type narrowing for union types (`string | number | boolean`).
3. **`formatCoordinate`**: Accepts a `readonly` tuple `[number, number, string]` and formats location strings safely.
4. **`concatenateArrays`**: Combines multiple arrays of generic type `T` using rest parameters.
5. **`getPopularCourses`**: Filters an array of courses implementing the `Course` interface without mutating the source data.
6. **`pluckValues`**: Generic utility leveraging the `keyof` constraint (`<T, K extends keyof T>`) to extract property values with index access types (`T[K][]`).
7. **`Employee` & `Manager` Classes**: Implements OOP inheritance using `protected` and `private` access modifiers with `super()`.
8. **`validateAgeAsync`**: Asynchronous function returning `Promise<string>`, resolving after 1000ms or rejecting with an `Error` instance.

---

## 📝 Technical Blog Posts

As part of the assignment requirements, two technical blogs have been written in clear, beginner-friendly English:

1. [**`any-unknown-never.md`**](./any-unknown-never.md)  
   *Question 2:* How TypeScript's type hierarchy works with `any`, `unknown`, and `never`, and why `unknown` is always preferred over `any`.

2. [**`generics-and-promises.md`**](./generics-and-promises.md)  
   *Question 4:* How generics work in TypeScript, and how they provide type safety when handling asynchronous `Promise<T>` responses.

---

## 🛠️ How to Compile & Run

To compile TypeScript files into JavaScript:

```bash
npx tsc
```

To run individual compiled solutions using Node.js:

```bash
node dist/solutions.js
```
