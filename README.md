# 🎬 Movie List App (Vue 3 + Bootstrap)

A small but intentional Vue 3 project that explores **state-driven UI flows**, user input validation, and dynamic rendering—without relying on external state managers or form libraries.

This project focuses on **understanding control flow and UI state**, not shipping a production app.

---

## 📌 What This Project Does

* Displays a list of movies with title, year, and rating
* Allows users to:

  * Add a movie step-by-step using a single input field
  * Remove a movie by title
  * Cancel an ongoing input flow at any point
* Dynamically updates:

  * Labels
  * Placeholders
  * Input types
  * UI visibility

All interactions are managed through **Vue 3’s Composition API**.

---

## 🧠 Key Concepts Practiced

* Vue 3 Composition API (`ref`, `reactive`)
* Conditional rendering (`v-if`)
* Event handling (`@click`, `@keyup.enter`)
* Controlled input with `v-model`
* Multi-step input workflows using internal state
* Basic validation logic tied to UI state
* Declarative rendering with `v-for`
* Bootstrap 5 utility-first styling

---

## 🏁 Milestones Achieved

* ✅ Built a complete CRUD-like flow without tutorials
* ✅ Implemented a single-input, multi-stage form pattern
* ✅ Avoided watchers and external libraries
* ✅ Used reactive state intentionally instead of ad-hoc variables
* ✅ Finished and polished the UI with Bootstrap
* ✅ Handled edge cases (empty input, invalid year/rating, missing movie)
* ✅ Maintained a clear separation between UI state and data state

Completion is the real milestone here.

---

## 🔍 Areas for Improvement (Next Iterations)

These are **deliberate omissions**, not oversights.

### 1. Refactor `inputVar` into Named States

Replace numeric flags with semantic constants or an enum-like object to improve readability and maintainability.

Example direction:

```js
const MODE = {
  IDLE: 0,
  ADD_TITLE: 1,
  ADD_YEAR: 2,
  ADD_RATING: 3,
  REMOVE: 4
}
```

---

### 2. Use Computed Properties for UI State

Some conditional logic (like when to show inputs or buttons) can be moved into computed properties instead of inline conditions.

---

### 3. Improve Validation Structure

Current validation is functional but sequential.
It could be extracted into reusable helper functions or a small validation layer.

---

### 4. Accessibility Improvements

* Associate `<label>` with `<input>` using `for` and `id`
* Improve keyboard navigation
* Add ARIA attributes where appropriate

---

### 5. Componentization

Extract parts into components:

* MovieTable
* MovieInput
* ActionButtons

This would make the app more scalable and testable.

---

## 🎯 Why This Repo Exists

This repository is not meant to impress with complexity.
It exists to document **learning, reasoning, and completion**.

It demonstrates:

* Cause-and-effect understanding of Vue reactivity
* Control over UI state
* Intentional design decisions
* The ability to finish and reflect

---

## 🚀 Tech Stack

* Vue 3 (CDN, Composition API)
* Bootstrap 5
* Vanilla JavaScript
* HTML5

---

## 📂 How to Run

Just open the HTML file in any modern browser.
No build step required.

---

## 📌 Final Note

Small, finished, and understood beats large, unfinished, and copied.

This project is one step in a longer path—and it documents that step honestly.

---
