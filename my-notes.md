# Epic React performance

- [Epic React performance](#epic-react-performance)
  - [Lesson 1 - Code Splitting](#lesson-1---code-splitting)
  - [Lesson 2 - useMemo For Expensive Calculations](#lesson-2---usememo-for-expensive-calculations)
  - [Lesson 3 - React.memo for Reducing Unnecessary Re-Renders](#lesson-3---reactmemo-for-reducing-unnecessary-re-renders)
  - [Lesson 4 - Window Large Lists with react-virtual](#lesson-4---window-large-lists-with-react-virtual)
  - [Lesson 5 - Optimize Context Value](#lesson-5---optimize-context-value)
  - [Lesson 6 - Fix "Perf Death by a Thousand Cuts"](#lesson-6---fix-perf-death-by-a-thousand-cuts)
  - [Lesson 7 - Production Performance Monitoring](#lesson-7---production-performance-monitoring)

## Lesson 1 - Code Splitting

- Dynamic module import syntax

```js
import('some/module/path').then(
  module => {
    // Do something with `module`
  },
  error => {
    // handle error
  },
)
```

- React Lazy Component Loading Syntax:

```jsx
const Fallback = <div>Loading</div>

// LazyComponent must be default export from import module
const LazyComponent = React.lazy(() => import('lazy/component/path'))

<React.Suspense fallback={Fallback}>
<LazyComponent/>
</React.Suspense>
```

## Lesson 2 - useMemo For Expensive Calculations

## Lesson 3 - React.memo for Reducing Unnecessary Re-Renders

## Lesson 4 - Window Large Lists with react-virtual

## Lesson 5 - Optimize Context Value

## Lesson 6 - Fix "Perf Death by a Thousand Cuts"

## Lesson 7 - Production Performance Monitoring
