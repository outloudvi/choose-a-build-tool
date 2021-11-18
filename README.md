
# Choose A Build Tool

A project to help developers select tools.

## There are ∞ compiler/bundler/packager/... !

There are just too many tools for a JavaScript developer. Here is a non-complete list:

-   [Babel](https://babeljs.io) - "The compiler for next generation JavaScript"
-   [Browserify](https://browserify.org/) - "lets you require('modules') in the browser by bundling up all of your dependencies"
-   [esbuild](https://esbuild.github.io/) - "An extremely fast JavaScript bundler"
-   [Grunt](https://gruntjs.com/) - "The JavaScript Task Runner"
-   [gulp.js](https://gulpjs.com/) - "A toolkit to automate & enhance your workflow"
-   [rollup.js](https://rollupjs.org/) - "Next-generation ES module bundler"
-   [Parcel](https://parceljs.org/) - "The zero configuration build tool for ..."
-   [Rome Toolchain](https://rome.tools/) - "A linter, compiler, bundler, and more ..."
-   [Snowpack](https://www.snowpack.dev/) - "The faster frontend build tool"
-   [swc](https://swc.rs/) - "Rust-based platform for the Web"
-   [Vite](https://vitejs.dev/) - "Next Generation Frontend Tooling"
-   [Webpack](https://webpack.js.org) - " A static module bundler for modern JavaScript applications"

But what **exactly** do they do? And how can I find a tool that can solve my problem?

That's why this project started. Check one or more pages below according to your requirements.

---

### If you want something to just automate your workflow...

You may want Grunt or gulp.js: [Workflow Automation](/workflow-automation/)

### If you want to just use some npm/Node.js package in browser...

Browserify is for you, or you may just use [esm.sh](https://esm.sh/): [Browser Package Bundler](/browser-package-bundler/)

### If you need to make you JavaScript code compatible on other environments...

For example, you are writting ES2021 but the clients of your might only support ES2018. In this case, what you need is a "transpiler" or "compiler" like Babel and swc: [Compiler](/compiler/)

### If you want a complete toolkit for web development...

Read until here, probably what you need is more than whichever we mentioned above. Then, you may want to check some all-in-one toolkits. They are usually called "bundler" in the past. Some of them may be modern and new, while some of them are well-famed and already widely used.

* [Webpack](https://webpack.js.org) and [rollup.js](https://rollupjs.org/) are two bundlers that have been used for really long. They may have the most complete set of plugins and StackOverflow questions, but somehow burdened by historic problems.
* [Snowpack](https://www.snowpack.dev/) comes with the ES Module and bundleless epoch. [ES Modules are generally supported by all recent browsers](https://caniuse.com/es6-module), which is the reason that Snowpack's solution works. It comes with faster speeds
* [Vite](https://vitejs.dev/) is somehow like Snowpack, but with some improvements that are useful for some developers ([There's also a comparison.](https://vitejs.dev/guide/comparisons.html#snowpack)). You might like using it if you are a Vue.js developer, since [Vite provides first-class Vue support](https://vitejs.dev/guide/features.html#vue).
* [Parcel](https://parceljs.org/) is the one that recently released its 2.0 and renamed from [`parcel-bundler`](https://www.npmjs.com/package/parcel-bundler). It natives support a wide range of languages including GraphQL, Rust and even GLSL.
* [esbuild](https://esbuild.github.io/) is trying to solve another problem with bundlers - JavaScript is still slow. To handle this, esbuild is written with Go, a lower-level language that is still comfortable to write (?).
* [Rome Toolchain](https://rome.tools/) and esbuild are alike. As of Rome, it initially aimes to do a lot, but it has pivoted to Rust-based from JavaScript-based, and [the rewrite is still in progress](https://rome.tools/blog/2021/09/21/rome-will-be-rewritten-in-rust).
