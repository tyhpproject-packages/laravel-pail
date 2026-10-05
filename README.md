<!-- tyhp-readme:start -->
# tyhpdef/laravel-pail

Tyhp type definitions for `laravel/pail` `1.2.7`.

```bash
composer require --dev tyhpdef/laravel-pail:1.2.7
```

This is a metapackage. Composer also installs `tyhpdef/laravel-pail-impl` (type files).
Require **this** name, not `tyhpdef/laravel-pail-impl`.

See https://tyhplang.com.

## Maintain `laravel/pail`? Ship the types yourself

If you are a Packagist maintainer of `laravel/pail`, you can take over these
types.

Copy `_tyhpdef/` from **`tyhpdef/laravel-pail-impl`** (Apache-2.0; keep the `NOTICE`).
Then either:

1. **Bundle** the files in `laravel/pail` and set `extra.tyhp.package` on
   that `composer.json`, plus
   `"replace": { "tyhpdef/laravel-pail": "self.version" }`, or
2. **Publish a sibling** types package under your vendor, versioned with
   `laravel/pail` (same `X.Y.Z`). Set `extra.tyhp.package` there,
   `require` `laravel/pail` with a real constraint,
   `"replace": { "tyhpdef/laravel-pail": "self.version" }`, and set
   `extra.tyhp.tyhpdef` on `laravel/pail` to your sibling’s Composer name.

Ship that to Packagist first, then open an issue:

https://github.com/tyhpproject/tyhp-runtime-src/issues/new?template=tyhpdef-ownership.yml

We verify Packagist ownership and that the types parse and cover the PHP
API, then stop publishing community tags for those versions. We do not
transfer the `tyhpdef/laravel-pail` Packagist name.

Full process: `TYHPDEF_OWNERSHIP.md` in
https://github.com/tyhpproject/tyhp-runtime-src
<!-- tyhp-readme:end -->
