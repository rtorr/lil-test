# lil-test

Occasionally, Ryan Florence likes to make my own testing framework

Context: https://twitter.com/ryanflorence/status/1162792430422200320

html:

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <meta http-equiv="X-UA-Compatible" content="ie=edge" />
    <title>Document</title>
  </head>
  <body>
    <script type="module">
      import { test, assert } from "https://cdn.pika.dev/lil-test-fw/v1";

      function sum(a, b) {
        return a + b;
      }

      test("dumb interview question", () => {
        const result = sum(5, 2);
        assert(result === 7, "sum");
      });
    </script>
  </body>
</html>
```

npm:

```bash
npm install lil-test-fw
```
