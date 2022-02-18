# Laravel Installation using Sail

## Install laravel using curl

```bash
curl -s "https://laravel.build/my-example-app" | bash
```

This command will install laravel inside my-example-app folder. Change as needed.

## Update Docker

If you run `sail up` and you get the following error it is likely that you need to update Docker Desktop.

```bash
ERROR: Service 'laravel.test' failed to build:
```

Before moving to the next step, check if there is any update to install for Docker Desktop and update it.

## Deploy laravel on Docker using `sail up` command

```bash
vendor/bin/sail up
```

It will take a minute then visit <http://localhost> and you should see your laravel application.

add an alias to run sail

```bash
alias sail='[ -f sail ] && bash sail || bash vendor/bin/sail'
```
