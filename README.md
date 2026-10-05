<!-- tyhp-readme:start -->
# tyhpdef/symfony-workflow

Tyhp type definitions for `symfony/workflow` `7.4.9`.

```bash
composer require --dev tyhpdef/symfony-workflow:7.4.9
```

This is a metapackage. Composer also installs `tyhpdef/symfony-workflow-impl` (type files).
Require **this** name, not `tyhpdef/symfony-workflow-impl`.

See https://tyhplang.com.

## Maintain `symfony/workflow`? Ship the types yourself

If you are a Packagist maintainer of `symfony/workflow`, you can take over these
types.

Copy `_tyhpdef/` from **`tyhpdef/symfony-workflow-impl`** (Apache-2.0; keep the `NOTICE`).
Then either:

1. **Bundle** the files in `symfony/workflow` and set `extra.tyhp.package` on
   that `composer.json`, plus
   `"replace": { "tyhpdef/symfony-workflow": "self.version" }`, or
2. **Publish a sibling** types package under your vendor, versioned with
   `symfony/workflow` (same `X.Y.Z`). Set `extra.tyhp.package` there,
   `require` `symfony/workflow` with a real constraint,
   `"replace": { "tyhpdef/symfony-workflow": "self.version" }`, and set
   `extra.tyhp.tyhpdef` on `symfony/workflow` to your sibling’s Composer name.

Ship that to Packagist first, then open an issue:

https://github.com/tyhpproject/tyhp-runtime-src/issues/new?template=tyhpdef-ownership.yml

We verify Packagist ownership and that the types parse and cover the PHP
API, then stop publishing community tags for those versions. We do not
transfer the `tyhpdef/symfony-workflow` Packagist name.

Full process: `TYHPDEF_OWNERSHIP.md` in
https://github.com/tyhpproject/tyhp-runtime-src
<!-- tyhp-readme:end -->
