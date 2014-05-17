Shadowsocks
========

Ansible role that installs the Shadowsocks secure SOCKS 5 proxy (http://shadowsocks.org). A random password is automatically chosen, and a QR code is generated that makes it easy to configure the iOS and Android clients.

Role Variables
--------------

Gathered facts are used to determine the default IPv4 address that the server should bind to. Make sure that gather_facts is not set to "no" in your playbook.

**Variables that can be set by the user (or another role)**

> shadowsocks_server_port: The port that the Shadowsocks server should listen on. Set to "8388" by default.

> shadowsocks_local_port: The local port that Shadowsocks should listen on. Set to "1080" by default.

> shadowsocks_timeout: Timeout (in seconds). Set to "600" by default.

> shadowsocks_encryption_method: The encryption method that will be used to secure the connection. A list of options can be found in the [Shadowsocks documentation](https://github.com/clowwindy/shadowsocks). The default for this role is "aes-256-cfb".

License
-------

The MIT License (MIT)

Copyright (c) 2014 Joshua Lund

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

Author Information
------------------

You can find me on [Twitter](https://twitter.com/joshualund), and on [GitHub](https://github.com/jlund/). I also occasionally blog at [MissingM](http://missingm.co).
