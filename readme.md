# global-asyncawaitpromise

One liner to add async/await and promises to your project

Check out [asyncawaitpromise](https://npmjs.com/package/asyncawaitpromise)
for a version that does not use globals

### Quickstart

    require('global-asyncawaitpromise')

    // Now we can use async/await and Promise
    const main = async(() => {
      console.log(3)
      await(Promise.delay(1000))
      console.log(2)
      await(Promise.delay(1000))
      console.log(1)
      await(Promise.delay(1000))
      console.log('🚀')
    })

    main()

### Docs

The following objects will be available globally

- [async](https://github.com/yortus/asyncawait)
- [await](https://github.com/yortus/asyncawait)
- [Promise](https://github.com/petkaantonov/bluebird)

### Why do I need this?

Because [callback hell](http://callbackhell.com) sucks, and it's
tedious to have to keep writing this boilerplate

    const Promise = require('bluebird')
    const async = require('asyncawait/async')
    const await = require('asyncawait/await')
