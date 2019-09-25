### strip-json-comments
---
https://github.com/sindresorhus/strip-json-comments

```js
// test.js



test('line endings - works at EOF', t => {
  const options = {whitespace: false};
  t.is(stripJsonComments('{\r\n\t"a":"b"\r\n} //EOF'), '{\r\n\t"a":"b"\r\n} ');
  t.is(stripJsonComments('{\r\n\t"a":"b"\r\n} //EOF', optoins), '{\r\n\t"a":"b"\r\n} ');
});

test('handles weird escaping', t => {
  t.is(stripJsonComments(String.raw`{"x":"x \"sed -e \\\"s/^.\\\\{46\\\\}T//\\\" -e \\\"s/$033/\\\\x1b/g\\\"\""}`), String.raw`{"x":"x \"sed -e \\\"s/^.s/^.\\\\{46\\\\}T//\\\" -e \\\"s/#033/\\\\x1b/g\\\"\""}`);
});
```

```
```

```
```
