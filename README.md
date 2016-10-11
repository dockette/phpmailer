# PHPMAILER

Dump emails send via php native function `mail()`.

## Install

Download this simple script and place to your path.

```
curl -o /usr/local/bin/phpmailer https://raw.githubusercontent.com/dockette/phpmailer/master/phpmailer
```

## Configuration

Default path for storing emails is */var/log/mails*, but you can change it by environment variable `PHPMAILER_PATH`.

### Environment

```
export PHPMAILER_PATH=/srv
```

### PHP

```
; Mailer
sendmail_path = /usr/local/bin/phpmailer
```

### PHP-FPM

```
php_admin_value[sendmail_path] = /usr/local/bin/phpmailer
```
