See [cypress/plugins/index.js](cypress/plugins/index.js). In this test we only allow tests with the string "#smoke" in the title. Thus other tests are automatically skipped.

When running in headless mode `npx cypress run` only a single test runs too

```text
  Running: spec.js...    (1 of 1)
picking tests from file cypress/integration/spec.js
found tests
[ [ 'suite', 'works A #smoke #regression' ],
  [ 'suite', 'works B #smoke'],
  [ 'suite', 'tests C #regression' ] ]


  suite
    ✓ works A #smoke #regression (18ms)
    ✓ works B #smoke (38ms)
    - tests C


  2 passing (81ms)
  1 pending
```

