https://awake-template.netlify.com/

Use the configuration below into nuxt config file:

```javascript
config.module.rules.push({
  enforce: 'pre',
  test: /\.(js|vue)$/,
  loader: 'eslint-loader',
  exclude: /(node_modules)/,
  options: { fix: true }
})
```

Important part is: options: { fix: true }

```javascript
extend(config, ctx) {
    if (ctx.dev && ctx.isClient) {
        config.module.rules.push({
            enforce : 'pre',
            test    : /\.(js|vue)$/,
            loader  : 'eslint-loader',
            exclude : /(node_modules)/,
            options : {
                fix : true
            }
        });
    }
}
```
