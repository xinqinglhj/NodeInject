# NodeInject
a inject tools for injecting js code into typora (with an activating script example)

### How it works:

1. unpack `node_modules.asar` package (in `Typora\resources`)
2. write `hook.js`  into `raven` package directory (raven will be required at the early stage of startup)
3. modify `index.js` of `raven`,injecting require of `hook.js`

> Currently using embedded javascript file (`hook.js`)

usage:

1. modify `hook.js` if you need
2. use `cargo build` to make  executable
3. Move the program to the Typora directory
4. run

### About `hook.js`

#### WARNING

JUST FOR LEARNING! 

SUPPORT GENUINE SOFTWARE AND DO NOT SELL PIRATED SOFTWARE !!!

#### Ability

- [x] make typora to activate with the generated activation code (Test passed in version 1.4.8 on windows)
- [x] hook `console.log` to remote http server and block override
- [x] hook `electron-fetch` for sniffing request
- [ ] Full version compatibility (Not tested for older version and may fail in the future)

