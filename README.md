# One Cache

> Server and client cache-first mechanism for avoiding API limits.

- You're developing against an API
- You don't want to be rate-limited 
- You're developing isomorphically or just don't care 😎

## Install

```sh
yarn add one-cache
```

## Usage

```javascript
let json = oneCache('my-users-cache', () => {
  return fetch('some-api.foo/users')
    .then(response => response.json())
})
```
