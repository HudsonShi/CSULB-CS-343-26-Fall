# Week 6 Lecture Pack: Front-End Fundamentals and Component Design

**Level:** Undergraduate software engineering · **Suggested class time:** 120 minutes

## Learning outcomes

Students can structure semantic HTML, apply responsive CSS layouts, explain state and props, build a reusable component, and conduct a basic usability test.

## 1. HTML communicates meaning

Semantic elements help browsers, assistive technology, search engines, and future developers understand a page.

```html
<header><h1>Library Catalog</h1></header>
<main>
  <section aria-labelledby="search-heading">
    <h2 id="search-heading">Find a book</h2>
    <form><label for="query">Title or author</label><input id="query" /></form>
  </section>
</main>
<footer>CS 343 demo</footer>
```

Use a button for actions, a link for navigation, and a label for every form input.

## 2. Layout with Flexbox and Grid

Flexbox is useful for one-dimensional alignment; Grid is useful when both rows and columns matter.

```css
.book-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(16rem, 1fr));
  gap: 1rem;
}
.toolbar { display: flex; justify-content: space-between; gap: .75rem; }
```

Responsive design starts with flexible content, readable line lengths, and touch-friendly targets—not merely shrinking a desktop screen.

## 3. Components are contracts

```mermaid
flowchart TD
    Page[Search page state] --> Search[SearchForm]
    Page --> Results[BookResults]
    Search --> Event[onSearch(query)]
    Event --> Page
    Page --> Props[results and loading props]
    Props --> Results
```

Props flow downward; user events flow upward. Keep a single owner for each important piece of state.

## 4. A reusable accessible button

```jsx
export function Button({ children, loading = false, ...props }) {
  return <button {...props} disabled={loading || props.disabled} aria-busy={loading}>
    {loading ? "Saving…" : children}
  </button>;
}
```

Test default, disabled, keyboard, loading, and error states. A component is reusable only if its behavior is predictable.

## 5. Usability testing in five steps

1. Define one task: “Borrow a book by author.”
2. Ask a participant to think aloud.
3. Observe without teaching.
4. Record evidence, not opinions.
5. Rank problems by severity and revise one design.

## In-class workshop (40 minutes)

Build a responsive card, input with error message, and modal. Swap laptops with a partner. The partner must complete a search using keyboard only and report one confusing interaction.

## Check for understanding

- Why is a clickable `<div>` usually worse than a `<button>`?
- Who should own the selected-book state: a modal or its page?
- When does Grid fit better than Flexbox?

## Homework

Publish a small component library with a README, screenshots, state examples, and an accessibility checklist.

## Suggested 18-slide teaching sequence

1. **Title and page critique** — Which parts of a webpage communicate meaning?
2. **Browser model** — HTML structure, CSS presentation, JavaScript behavior.
3. **Semantic HTML** — Header, navigation, main, section, article, footer.
4. **Form accessibility** — Labels, error text, focus order, and keyboard use.
5. **CSS cascade** — Explain selectors, inheritance, and specificity briefly.
6. **Box model** — Content, padding, border, and margin visual exercise.
7. **Flexbox** — Align a search toolbar in one dimension.
8. **Grid** — Build responsive book cards in two dimensions.
9. **Responsive design** — Use constraints and breakpoints thoughtfully.
10. **Modern JavaScript** — Variables, functions, objects, arrays, async requests.
11. **Component mindset** — Repetition becomes a reusable contract.
12. **Props and state** — Trace data down and event callbacks up.
13. **Accessible button demo** — Inspect disabled and loading semantics.
14. **Design-system states** — Default, hover, focus, disabled, error, loading.
15. **Usability test method** — Observe a task without coaching.
16. **Component build studio** — Card, input, modal, responsive layout.
17. **Keyboard peer test** — Collect evidence of a confusing interaction.
18. **Exit ticket** — Replace one non-semantic element with the correct HTML.
