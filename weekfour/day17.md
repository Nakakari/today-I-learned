# Day Seven Ten

## What I've learn?
<aside>
🔑 What is the main difference between `useCallback` and `useMemo`? And when to use `useCallback` of React Hooks?

</aside>

`useMemo(() => (bar) => foo + bar, [foo]);`

Equivalent code with useCallback:

`useCallback((bar) => foo + bar, [foo]);`

Use callback is **just a shorthand** variation of `useMemo` to use with functions. 

Here is why it exists: When you use `useMemo`, the value usually changes when one of its dependencies changes. For example:

`const fullName = useMemo(() => firstName + lastName, [firstName, lastName]);`

Here, when `firstName`or `lastName`change, we don't need to have a completely different function with a different body, but we do need to have a new instance of the same function so that it has up to date values in closure (dependencies). So React team just added it for convenience as it is a common use case, and the `() => () =>`syntax is somewhat ugly.