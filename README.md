<!-- tyhp-readme:start -->
# tyhpdef/phpstan-phpstan-phpunit

Tyhp type definitions for `phpstan/phpstan-phpunit` `2.0.18`.

```bash
composer require --dev tyhpdef/phpstan-phpstan-phpunit:2.0.18
```

This is a metapackage. Composer also installs `tyhpdef/phpstan-phpstan-phpunit-impl` (type files).
Require **this** name, not `tyhpdef/phpstan-phpstan-phpunit-impl`.

See https://tyhplang.com.

## Maintain `phpstan/phpstan-phpunit`? Ship the types yourself

If you are a Packagist maintainer of `phpstan/phpstan-phpunit`, you can take over these
types.

Copy `_tyhpdef/` from **`tyhpdef/phpstan-phpstan-phpunit-impl`** (Apache-2.0; keep the `NOTICE`).
Then either:

1. **Bundle** the files in `phpstan/phpstan-phpunit` and set `extra.tyhp.package` on
   that `composer.json`, plus
   `"replace": { "tyhpdef/phpstan-phpstan-phpunit": "self.version" }`, or
2. **Publish a sibling** types package under your vendor, versioned with
   `phpstan/phpstan-phpunit` (same `X.Y.Z`). Set `extra.tyhp.package` there,
   `require` `phpstan/phpstan-phpunit` with a real constraint,
   `"replace": { "tyhpdef/phpstan-phpstan-phpunit": "self.version" }`, and set
   `extra.tyhp.tyhpdef` on `phpstan/phpstan-phpunit` to your sibling’s Composer name.

Ship that to Packagist first, then open an issue:

https://github.com/tyhpproject/tyhp-runtime-src/issues/new?template=tyhpdef-ownership.yml

We verify Packagist ownership and that the types parse and cover the PHP
API, then stop publishing community tags for those versions. We do not
transfer the `tyhpdef/phpstan-phpstan-phpunit` Packagist name.

Full process: `TYHPDEF_OWNERSHIP.md` in
https://github.com/tyhpproject/tyhp-runtime-src
<!-- tyhp-readme:end -->
