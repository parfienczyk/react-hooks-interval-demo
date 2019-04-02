# react-hooks-interval-demo

1. Functional updates for useState

```javascript
useEffect(() => {
  const interval = setInterval(() => {
    setCount(c => c + 1);
  }, 500);
  return () => clearInterval(interval);
}, []);
```


2. setTimeout

```javascript
useEffect(() => {
  const timeout = setTimeout(() => {
    setCount(count + 1);
  }, 500);
  return () => clearTimeout(timeout);
}, [count]);
```

#### check:
https://medium.com/@sdolidze/the-iceberg-of-react-hooks-af0b588f43fb
