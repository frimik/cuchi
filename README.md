# tunnlea

``tunnlea``, pronounced `/ˈtʌnliː/` is a fork of [cuchi](https://github.com/michlabs/cuchi)

## Install tunnlea

    $ go install github.com/frimik/tunnlea

## Usage

`tunnlea` binary runs in both server and client mode

```sh
# tunnlea_server
$ tunnlea -s backend_interface:1203 frontend_interface:80

# tunnlea_client
$ tunnlea tunnlea_server:1203 localhost:8080 myhost.example.com
```

Then the request to `myhost.example.com` will be tunnelled to `localhost:8080`.

## License

BSD