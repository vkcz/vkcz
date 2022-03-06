### Hi there 👋

The following JS function provides the sum of the letters in some text (`a = 1`, `b = 2`, ... `z = 26`):
```js
lettersum = t => t.toLowerCase().split("").filter(s => s.match(/[a-z]/)).map(l => l.codePointAt(0) - 96).reduce((a, b) => a + b);
```

This one computes <var>b</var><sup><var>e</var></sup> mod <var>m</var>:
```js
modpow = (b, e, m) => {
    let r = 1;
    while (e > 0) {
        r = (r * b) % m;
        e--;
    }
    return r;
};
```

The following, using those functions, with the two primary parts of my name in place of `"text"`, outputs `1141`:
```js
const s = lettersum("text");
console.log(modpow(s, s, 8191));
```

<!--
**vkcz/vkcz** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
