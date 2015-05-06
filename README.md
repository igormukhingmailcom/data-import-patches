# data-import-patches

This repository collect useful patches for [ddeboer/data-import](https://github.com/ddeboer/data-import) in form prepared for automatically apply via [netresearch/composer-patches-plugin](https://github.com/netresearch/composer-patches-plugin).

It is almost for internal usage as at this time consists only from my own patches. But you can use it if you found it useful.

## Usage

At this time, there are two patches groups available - for `master` branch and for `0.18.0` release.

### 0.18.0

To use patches for latest stable version of [data-import:0.18.0](https://github.com/ddeboer/data-import/tree/0.18.0) you need configure your composer.json like that:

```json
{
    "repositories": [
        {
            "type": "vcs",
            "url": "https://github.com/igormukhingmailcom/data-import-patches.git"
        }
    ],

    "require": {
        "netresearch/composer-patches-plugin": "1.1.*@dev",

        "ddeboer/data-import": "0.18.0",
        "igormukhingmailcom/data-import-patches": "dev-master",
    }
}
```

### Master

All patches for [data-import:master](https://github.com/ddeboer/data-import/tree/master) branch added to master branch of this repository and deleted once it merged with stream repository.

```json
{
    "repositories": [
        {
            "type": "vcs",
            "url": "https://github.com/igormukhingmailcom/data-import-patches.git"
        }
    ],

    "require": {
        "netresearch/composer-patches-plugin": "1.1.*@dev",

        "ddeboer/data-import": "dev-master",
        "igormukhingmailcom/data-import-patches": "dev-master",
    }
}
```

## License

MIT
