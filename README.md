# NetCore-TS-Knockout-Webpack

Lab for optimised runtime changes from TypeScript /w KnockoutJS trough WebPack to output under .NET Core

## Hierarchy

```bash
TestA
├──:TestABase
│  ├──TestC
│       ├──:TestCBase
├──Shared
    ├──Shared2
        ├──Shared3
TestB
├──TestC
│  ├──:TestCBase
├──Shared3
```

## Bundling

Common will contain all shared classes between all endpoints
```bash
Common.js
├──TestC
├──TestCBase
├──Shared3
```

TestA will contain all specific classes for endpoint TestA
```bash
TestA.js
├──TestA
├──TestABase
├──Shared
├──Shared2
```

TestB will contain all specific classes for endpoint TestB
```bash
TestB.js
├──TestB
```

Vendors will be bundeled by vendor name
vendor.jquery.js
vendor.knockout.js
vendor.webpack.js