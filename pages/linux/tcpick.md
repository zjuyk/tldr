# tcpick

> Packet sniffing and network traffic analysis tool.
> It can capture and display TCP connections and data. It can also monitor network traffic on a interface, host, or port.
> More information: <https://manned.org/tcpick.8>.

- Capture traffic on a specific interface, port and host::

`sudo tcpick {{[-i|--interface]}} {{interface}} {{[-C|--colors]}} -h {{host}} -p {{port}}`

- Capture traffic on port 80 (HTTP) of a specific host:

`sudo tcpick {{[-i|--interface]}} {{eth0}} {{[-C|--colors]}} -h {{192.168.1.100}} -p {{80}}`

- Display help:

`tcpick --help`
