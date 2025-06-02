# README
A course on penetration testing in Haaga-Helia. [Tunkeutumistestaus](https://terokarvinen.com/tunkeutumistestaus/)

## Topics covered during the course
### h1:

* **Nmap port scanning**: `nmap -T4 -A`, OS/service detection, filtered vs. open ports, `-p` and timing templates
* **Network isolation for safe testing**: VirtualBox & Vagrant use, NAT vs. Host-Only
* **VM targets**: Kali, Metasploitable2/3, Apache2, Salt-master
* **Kill Chain phases**: Recon, Delivery, Exploitation, etc.
* **Legal case analysis**: Finnish court case on scanning

### h2:

* **OWASP Top 10**

* **Web exploitation tools**:
  * **Burp Suite**: Intercept, modify, replay requests
  * **ZAP proxy** + FoxyProxy: Pattern-based interception

* **Attack techniques**:
  * Reflected and stored XSS
  * Path traversal (simple, bypass, absolute)
  * IDOR
  * SSRF
  * SSTI (Django-specific, info disclosure)

* **Encoding/decoding**: `pencode`, URL and Base64 chaining

### h3:

* **FFUF for fuzzing**:
  * Directory discovery, file extension brute force
  * Recursion, parameter mining, host header fuzzing (virtual hosts)
  * Bypass noisy 404s (response size filtering)
  * Rate-limiting evasion (delay + threads)
  * Encoder chaining (`-enc`, piping through md5)

### h4:

* **Password cracking**:
  * `hashcat`: MD5, SHA256, SHA512crypt
  * `john`: PKZIP, 7z (via zip2john / 7z2john)

* **Payload creation**:
  * `msfvenom`: Meterpreter reverse shells (ELF payloads)

* **Post-exploitation**:
  * Listener setup (`multi/handler`)
  * Reverse connection from victim
