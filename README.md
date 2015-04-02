# find-port

Find open ports programmatically.

# Usage

The `port-open-p` function takes an integer and determines whether a port by
that number is open.

The `find-port` function, by default takes no arguments, and returns an open
port. Two keyword arguments, `:min` and `:max`, may be given to constrain the
port range in which to search for ports.

By default, the range is from 49152 to 65535. This is the range
[recommended][range] by the [Internet Assigned Numbers Authority][iani] for use
in private or ephemeral ports, since this function will probably be used e.g. to
pick an open port for testing, rather than to pick a port to run a production
server on.

[range]: http://www.iana.org/assignments/service-names-port-numbers/service-names-port-numbers.xhtml
[iani]: http://www.iana.org/

# License

Copyright (c) 2015 Fernando Borretti

Licensed under the MIT License.
