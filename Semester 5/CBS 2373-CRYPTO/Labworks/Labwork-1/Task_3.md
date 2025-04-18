# **Sniff Network Traffic**
In this lab, we will be sniffing the traffic of ftp, ssh, telnet, and http using wirieshark.

## Process 
To start the sniffing, we need to log in to the service first.
1. FTP
    ```bash
    ftp 192.168.193.137
    ```
    Result:
    ![ftp](Screenshots/ftp.png)

2. TELNET 
    ```bash
    telnet 192.168.193.137
    ```
    Result:
    ![telnet](Screenshots/telnet.png)

3. SSH
    ```bash
    ssh -oHostKeyAlgorithms=+ssh-rsa msfadmin@192.168.193.137
    ```
    Result:
    ![ssh](Screenshots/ssh.png)

4. HTTP
    - Do the same thing as we brute force the website while open the wireshark. 

### Wireshark 

1. FTP
    - filter using **ftp** or  **tcp.port == 21** . 
    Result:
    ![ftp](Screenshots/wireshark-ftp.png)

2. TELNET
    - filter using **telnet** or **tcp.port == 23** .
    Result:
    ![telnet](Screenshots/wireshark-telnet.png)

3. SSH
    - filter using **ssh** or **tcp.port == 22** .
    Result:
    ![ssh](Screenshots/wireshark-ssh.png)

4. HTTP
    - filter using **http** .
    Result:
    ![http](Screenshots/wireshark-http.png)
