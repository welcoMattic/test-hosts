# Test hosts

This is a test-case for https://github.com/symfony/symfony/pull/36187

To run it:

- Clone the repo
- Run `composer install`
- Clone Symfony repo in another dir and run from it `./link ../test-hosts` to replace vendor/symfony with symlinks from Symfony cloned repo
- Add `127.0.0.1 example.test en.example.test nl.example.test` to your `/etc/hosts` file
- Run `symfony proxy:start`
- Configure your system to use the proxy like described [here](https://symfony.com/doc/current/setup/symfony_server.html#local-domain-names)
- Run `symfony serve`
- Visit `https://example.test`
