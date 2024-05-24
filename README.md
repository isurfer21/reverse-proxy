# reverse-proxy

> A simple reverse-proxy server with zero third-party module dependency

It is a zero-dependency basic reverse-proxy that can be used to improve the performance, security, and scalability of your web applications.

## Prerequisite

It requires [node.js](https://nodejs.org/) to be installed on the system.

## Install

To install this module, run the following command:

```sh
npm install reverse-proxy-ws
```

**Note**: Since it doesn't require any third-party module, so there is no need to build it. You can run it right away!

### CLI Options

This module can be run from the command line with the following options:

| Short | Long Options       | Description                                        |
|-------|--------------------|----------------------------------------------------|
| `-h`  | `--help`           | Display help menu                                  |
| `-a`  | `--addr=HOST`      | Provide server host address (default: `127.0.0.1`) |
| `-p`  | `--port=PORT`      | Provide server port (default: `8080`)              |
| `-c`  | `--conf=FILE_PATH` | Provide proxies configuration file path            |

## Prepare

Ensure this reverse proxy app is installed globally as a standalone command.

Modify the routes defined in the default `proxy-config.json` according to your need.

## Execute

Refer the below provided examples to use this app from the command-line.

To display help menu, execute this command

```sh
reverse-proxy --help
```

To run the reverse proxy server on host `127.0.0.1` and port `8081` using the proxies configuration file `proxy-config.json`, execute this command

```sh
reverse-proxy --addr=127.0.0.1 --port=8081 --conf=proxy-config.json
```

Alternatively, to use shorthand options in the previous command, execute this command

```sh
reverse-proxy -a=0.0.0.0 -p=8080 -c=proxy-config.json
```

## License

This module is licensed under the **MIT License**. See the [LICENSE](./LICENSE) file for more information.