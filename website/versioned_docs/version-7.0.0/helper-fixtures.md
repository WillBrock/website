---
id: version-7.0.0-babel-helper-fixtures
title: @babel/helper-fixtures
sidebar_label: babel-helper-fixtures
original_id: babel-helper-fixtures
---

## Usage

```javascript
import getFixtures from "@babel/helper-fixtures";

type TestFile = {
  loc: string;
  code: string;
  filename: string;
};

type Test = {
  title: string;
  disabled: boolean;
  options: Object;
  exec: TestFile;
  actual: TestFile;
  expected: TestFile;
};

type Suite = {
  options: Object;
  tests: Array<Test>;
  title: string;
  filename: string;
};

let fixtures: Array<Suite> = getFixtures("/User/sebmck/Projects/babel-something/test/fixtures");
```

