# LXI - SpartaCodingClub Full-Stack Bootcamp in Indonesia] 2022/11/01 TIL/Week 3

## What I Learn Today?

Well, I learned more deeply about the different between useState and useEffect.

```kotlin
    To put it simply, both `useState` and `useEffect` enhance functional components to make them do things that classes can but functional components (without hooks) cannot:

    - `useState` allows functional components to have **state**, like `this.state` in class components.
    - `useEffect` allows functional components to have **lifecycle methods** (such as `componentDidMount`, `componentDidUpdate` and `componentWillUnmount`) in one single API.
    - When a function is passed to `useState`, this is signaling to React to use [lazy initialization](https://reactjs.org/docs/hooks-reference.html#lazy-initial-state) - the function will be invoked to calculate the initial value only when the component mounts. If the value to be put into state can be calculated/retrieved *synchronously*, this is probably the best design pattern to use - it's short and doesn't require you to later differentiate between whether the state value is undefined or populated.
    - The time to use `useEffect`is when the value to be populated *can't* be computed synchronously, in which case the best approach is to have both `useState`  (for the state) and `useEffect`(to indicate that you want to run a function to retrieve the state value just once).

    When we implemented `React.useState(() =>getMovies(), [])`, `useEffect`is more suited for the task because it doesn't have a return value (unlike `useState`), and is more flexible, because it does accept a dependency array. `useEffect`much more clearly indicates to readers of the code "This callback should run only when the dependency array changes."
```

## What did I do Well?

I had been enjoying to disscuss with members in my team. We talk about ReactJS data flow with unidirectional flow (one-way). The other data flow system is Bi-directional.

All can be seen in:

[![forthebadge](../Images/weektwo/logo192.png)](https://teamsparta.notion.site/Team-7-Team-Task-Notion-Page-8ff233392ba0447e82b7cba6bf21d55d)

## What Needs to Improve?

To know more about React basic components and rules.

## Documentation

![title](../Images/weekthree/12.png)