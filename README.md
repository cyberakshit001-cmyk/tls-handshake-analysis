## TLS Handshake Analysis (HTTPS)

### Objective
To analyze how HTTPS establishes a secure connection using TLS.

### Tools
Wireshark, Google Chrome

### Observations

#### Client Hello
The browser advertises supported cipher suites including AES-GCM.


#### Server Hello
The server selects AES-GCM as the encryption algorithm.

#### Key Exchange
ECDHE was used, providing Perfect Forward Secrecy.


### Security Impact
AES-GCM encrypts and authenticates data.  
ECDHE ensures every session has a unique secret key, preventing past traffic from being decrypted.
