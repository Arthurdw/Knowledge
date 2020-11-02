# Network Communication

Short description

## Keywords

These abbreviations are used in the text.

| Abbreviation | Definition                          |
| ------------ | ----------------------------------- |
| IP           | Internet Protocol                   |
| DHCP         | Dynamic Host Configuration Protocol |
| DNS          | Domain Name System                  |
| ISP          | Internet Service Provider           |
| OSI          | Open Systems Interconnection        |

## Ip Adresses

### What are IP adresses?

In short an IP adress is a network adress for your computer so that the internet knows where data came from or to where it has to go to.

You can see it as your street adress, but for your computer.

Every device that is connected to the internet has a IP adress.

### Types of IP's

#### IPv4

The most common type of IP adress is known as a IPv4 (version 4). An IPv4 consists of four numbers, each number is between **0** and **255** and gets delimited by a single dot.

```js
140.82.121.4
```

#### IPv6

The new IP adress is IPv6 (version 6). An IPv6 consists of 8 groups of 4 hexadecimal *[`0123456789abcdef`]* digits and is delimited by a colon.

```py
2a00:1450:400e:0800:0000:0000:0000:200e
```

But an IPv6 has some different notation rules. It can omit leading zeros.

```py
2a00:1450:400e:800:0:0:0:200e
```

And a double colon can be used to replace a series of zeroes, for example.

```py
2a00:1450:400e:800::200e
```

### What happens if we run out of IPs?

It has already happend, since and IPv4 can only have around 4.3 billion unique IP adresses we ran out. The IPv4 format wasn't designed for the amount of IPs that get used today. 

Fortunately there is IPv6 which can handle enough IPs for the future. *(Hopefully?)* *[IPv6 max: `340,282,366,920,938,463,463,374,607,431,768,211,456`]*

#### How do I get my IP?

**DHCP** is something your **ISP** uses to provide IPs to its hosts. *(Hosts are devices/users)*

#### If we use IPs to visit the internet how can I just type example.com?

The **DNS** servers handle this, these have records that contain the domain and the corresponding IP adress. *(This includes subdomains)*

## PORTs

Since you only have one IP adress to communicate on the internet you would not be able to let multiple services connect to the internet at the same time with the same IP as that the data that gets received from the internet would have no idea to which program it has to go. Thats why they invented PORTS, a port is basically a way for your computer to know to where it has to send the received data. And yes thats not a mistake, it says computer. As a port is on layer 3 or 4 on the OSI model it doesn't get opened by the first layer. 

In short, ports are a way to let your computer have multiple services communicating on the internet at once.

#### Privileged ports and protocols

| Port     | Abbreviation | Definition                          |
| -------- | ------------ | ----------------------------------- |
| 21       | FTP          | File Transfer Protocol              |
| 22       | SSH          | Secure Shell                        |
| 23       | Telnet       | Telnet                              |
| 25       | SMTP         | Simple Mail Transfer Protocol       |
| 53       | DNS          | Domain Name System                  |
| 67, 68   | DHCP         | Dynamic Host Configuration Protocol |
| 69       | TFTP         | Trivial File Transfer Protocol      |
| 80       | HTTP         | Hypertext Transfer Protocol         |
| 110      | POP3         | Post Office Protocol                |
| 139, 445 | SMB          | Server Message Block                |
| 143      | IMAP         | Internet Message Access Protocol    |
| 161      | SNMP         | Simple Network Management Protocol  |
| 443      | HTTPS        | Hyper Text Transfer Protocol Secure |

# 
