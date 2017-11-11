<% const camelcasedName = this.camelcase(name) -%>

<div class="text-xs-center" align="center" style="margin: 20px">
  <img src="./docs/banner.svg" height="255" alt="<% name %>">
</div>

<div class="text-xs-center" align="center">

<!-- [![vue2](https://img.shields.io/badge/vue-2.x-brightgreen.svg)](https://vuejs.org/) -->
[![NPM version](https://img.shields.io/npm/v/<%= name %>.svg?style=flat)](https://npmjs.com/package/<%= name %>)
[![NPM downloads](https://img.shields.io/npm/dm/<%= name %>.svg?style=flat)](https://npmjs.com/package/<%= name %>)
[![CircleCI](https://circleci.com/gh/<%= username %>/<%= name %>/tree/master.svg?style=shield)](https://circleci.com/gh/<%= username %>/<%= name %>/tree/master)
<% if (coverage) { %>[![codecov](https://codecov.io/gh/<%= username %>/<%= name %>/branch/master/graph/badge.svg)](https://codecov.io/gh/<%= username %>/<%= name %>)<% } %>

</div>

## Introduction
<%= description %>

## Install

```bash
<% if (pm === 'yarn') { %>yarn add<% } else { %>npm i<% } %> <%= name %>
```

## Usage

```js
const <%= camelcasedName %> = require('<%= name %>')

...
```

## Contributing

Please read [CONTRIBUTING.md](CONTRIBUTING.md) for details on our code of conduct, and the process for submitting pull requests to us.

## Versioning

We use [SemVer](http://semver.org/) for versioning. For the versions available, see the [tags on this repository](https://github.com/znck/prop-types/releases).

## Author

**<%= name %>** © [<%= author %>](https://github.com/<%= username %>), Released under the [MIT](./LICENSE) License.<br>
Authored and maintained by <%= author %> with help from contributors ([list](https://github.com/<%= username %>/<%= name %>/contributors)).

> [<%= website.replace(/^https?:\/\//, '') %>](<%= website %>) · GitHub [@<%= author %>](https://github.com/<%= username%>)<% if (twitter) { %> · Twitter [@<%= twitter %>](https://twitter.com/<%= twitter %>)<% } %>
