# braadiv/dom-crawler

> **⚠️ This is a PHP 8.4 compatibility fork — NOT an original work.**

## Credits & Attribution

This package is a **modernized fork** of the original [`symfony/dom-crawler`](https://github.com/symfony/dom-crawler.git), created and maintained by **Fabien Potencier and the Symfony Community**.

**All original code, design, and intellectual property belong to the original author(s).**

The only modifications made in this fork are:
- Fixing PHP 8.4 deprecation warning (`implicit nullable parameter` in `Crawler::form()`)
- Replacing deprecated `mb_convert_encoding($content, 'HTML-ENTITIES', ...)` with `mb_encode_numericentity(...)`
- Updating `composer.json` to support PHP 8.1–8.4 LTS
- Adding `"replace": {"symfony/dom-crawler": "self.version"}` as a drop-in replacement
- Retaining 100% backward compatibility as a drop-in replacement

---

## Why this fork?

The Symfony 3.4 component series reached End-of-Life and is no longer updated by the Symfony core team. However, legacy packages and Yii2 extensions (such as `wbraganca/yii2-dynamicform`) still pin their dependencies to `~2.8|~3.0`. Under PHP 8.4 LTS, implicit nullable parameters trigger `E_DEPRECATED` warnings.

This fork provides a **safe, drop-in replacement** under PHP 8.4 without altering any runtime behaviour.

---

## Installation

```bash
composer require braadiv/dom-crawler
```

## Original Package Information

| | |
|:--|:--|
| **Original Package** | [`symfony/dom-crawler`](https://github.com/symfony/dom-crawler) |
| **Original Version** | `v3.4.47` |
| **Original Authors** | Fabien Potencier, Symfony Community |
| **Original License** | `MIT` |
| **Fork Maintainer** | `braadiv` ([github.com/braadiv](https://github.com/braadiv)) |
| **PHP Compatibility** | `>=8.1 || ^8.2 || ^8.3 || ^8.4` |

---

## Changes from Original

See [CHANGELOG.md](../CHANGELOG.md) for a detailed list of all modifications.

---

## License

This fork retains the **same license** as the original package (`MIT`).
All rights and credits belong to the original authors.
