# WP-CLI Hacks

## Config

Look up `wp-config.php`

```
wp config get
```

Look up `wp-config.php` path

```
wp config path
```
Look up size of db tables in MB

## DB

```
wp db size --size_format=mb --tables
```

## Core

Look up core version

```
wp core version
```

Verify core checksums

```
wp core verify-checksums
```

Update core to specific version

```
wp core update --version=5.0.1
```

Check if core is up to date

```
wp core check-update
```

## Package

Install package

```
wp package install trepmal/wp-revisions-cli
wp package install dereckson/wp-cli-polylang
```

## Revisions

List all revisions

```
wp revisions list
```

List all revisions of a specific post

```
wp revisions list --post_id=300
```

Clean all revisions before a specific date

```
wp revisions clean --before-date=2019-01-01
```

## Scaffold

Create plugin

```
wp scaffold plugin --prompt
```

Create theme

```
wp scaffold theme --prompt
```

Create child theme

```
wp scaffold child-theme --prompt
```