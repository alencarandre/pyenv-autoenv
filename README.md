# pyenv-autoenv

This is helpful to manage virtual environment automatically. Just enter the project directory via bash and the virtual environment will be set to you.

## Instalations

1. **Check if dependencies are installed**
    - [pyenv](https://github.com/pyenv/pyenv)
    - [pyenv-virtualenv](https://github.com/pyenv/pyenv-virtualenv)
    - [Git](https://git-scm.com/)

2. **Check out pyenv-autoenv into plugin directory**

    ```sh
    $ git clone https://github.com/alencarandre/pyenv-autoenv.git $(pyenv root)/plugins/pyenv-autoenv
    ```

3. Add pyenv autoenv-init to your shell to enable auto-activation of virtualenvs.

    ```sh
      $ echo 'eval "$(pyenv autoenv init)"' >> ~/.bash_profile
    ```

## Usage


### Create `.pyenv-virtualenv` file

Inside your project root path, run command bellow:

```sh
$ pyenv autoenv your-virtual-environment-name-here
```

### Check version

```sh
$ pyenv autoenv version
```

### Upgrade to last version

```
$ pyenv autoenv upgrade
```

## Limitation and contribution

This plugin was tested only for `bash`. If you need to use in other terminals, fell free to test and go ahead to implement or fix something if necessary. Your contribution is thankful.

## Licence

The gem is available as open source under the terms of the [MIT License](https://opensource.org/licenses/MIT).
