# Week 6 — Accessible React Button

```jsx
export function Button({ children, loading = false, ...props }) {
  return (
    <button {...props} disabled={loading || props.disabled} aria-busy={loading}>
      {loading ? "Saving…" : children}
    </button>
  );
}
```

Use a real `<button>` so keyboard focus, disabled state, and semantics are available by default.
