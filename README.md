## Getting Started

1. Fork the codesandbox from https://codesandbox.io/p/devbox/mh3vtj
2. Run the development server:

```bash
yarn dev
```

## Exercises

Feel free to use [nextjs](https://nextjs.org/)'s official documentation to help with the exercise. If you are stuck at an exercise, you can move on to the next one.

### Routing

Add the following routes to the app

a. `/about`

b. `/<name>/info`. For example,

- `/calif/info` will show a blank page with "Calif" text
- `/xyz/info` will show "Xyz"

### Eslint rules

Currently, `Image` component imported in `app/page.tsx` is not used. However, `yarn lint` does not yield any warning or error.

```
import Image from "next/image";

export default function Home() {
  return (
    <main>
      Home Page
    </main>
  );
}
```

Why? If possible, please fix or show an approach to fix the issue. The fix isn't simply removing the `import`. We want error/warning so we can prevent similar pattern in the future.

### Unit tests

Write unit tests to confirm the followings

a. `Home` component that it has "Home Page"
b. Bonus: test route `<name>/info`
