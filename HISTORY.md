# History

## 2023-03-03

* Add Bootstrap v5.2.3

```bash
$ VERSION='5.2.3'
curl -LOk "https://github.com/twbs/bootstrap/archive/v${VERSION}.zip"
unzip "v${VERSION}".zip
rm -rf site/themes/jamesbond-world/assets/scss/bootstrap
mv "bootstrap-${VERSION}/scss" site/themes/jamesbond-world/assets/scss/bootstrap
rm -rf bootstrap-${VERSION} "v${VERSION}".zip
```

## 2023-03-02

* Create a new Hugo site

```bash
$ hugo new theme jamesbond-world
...
```

* Create a new Hugo site

```bash
$ hugo new site site
...
```

* Aggregate and copy shared files.

```bash
$ ./scripts/004-shared
...
```

## 2023-02-23

* Modify covers for EPUB files.

```bash
$ ./scripts/003-covers
...
```

## 2023-02-17

* Download original EPUB files from https://www.fadedpage.com.

```bash
$ ./scripts/000-download
...
```

* Unzip original EPUB files.

```bash
$ ./scripts/001-unzip
...
```

* Zip extracted files to EPUB files.

```bash
$ ./scripts/002-zip
...
```
