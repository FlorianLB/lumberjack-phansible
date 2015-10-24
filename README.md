# Lumberjack Phansible

Based on [Phansible](https://github.com/phansible/phansible) and customized for CleverAge needs.

[Phansible](http://phansible.com) is a simple generator for Vagrant projects, targeting PHP development environments, using Ansible as Provisioner.

## Setup

- Clone the repo: ```git clone https://github.com/Phansible/phansible.git```
- Go into the phansible folder ```cd phansible/```
- Install the dependencies with [composer](https://getcomposer.org/): ```php composer install```
- Run the php built in server: ```php -S 0.0.0.0:8080 -t web/```
- You can now go on [http://localhost:8080](http://localhost:8080) to see your modification.

As an alternative, you can also use the included Vagrant setup (requires Ansible).

## Tests
To run the tests just do:
```
 ./vendor/bin/phpunit
```

## Code style
To check the code style just do:
```
 ./vendor/bin/phpcs --standard=psr2 ./src
 ./vendor/bin/phpmd src/ text codesize,controversial,design,naming,unusedcode
```

When no errors appear you are ready to push your commits!
