```console
$ 04_02_parse_derive --help
clap [..]
A simple to use, efficient, and full-featured Command Line Argument Parser

Usage:
    04_02_parse_derive[EXE] <PORT>

Arguments:
    <PORT>    Network port to use

Options:
    -h, --help       Print help information
    -V, --version    Print version information

$ 04_02_parse_derive 22
PORT = 22

$ 04_02_parse_derive foobar
? failed
error: Invalid value "foobar" for '<PORT>': invalid digit found in string

For more information try --help

$ 04_02_parse_derive 0
? failed
error: Invalid value "0" for '<PORT>': 0 is not in 1..=65535

For more information try --help

```