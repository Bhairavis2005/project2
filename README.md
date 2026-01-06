# project2
# Network Traffic Analysis using Wireshark (Kali Linux)

## 1. Introduction

This project focuses on practical network traffic analysis using **Wireshark** on **Kali Linux**. The aim of this work is to understand how data travels over a network and how different protocols such as HTTP, HTTPS, DNS, and ICMP can be observed and analyzed in real time.

This project was performed in a controlled environment for learning and academic purposes only.

---
## 2. Objective
The main objectives of this project are:
* To capture live network traffic using Wireshark
* To analyze different types of network protocols
* To understand the difference between secure and insecure communication
* To identify basic suspicious or unusual traffic patterns
---
## 3. Tools and Environment Used
* Kali Linux
* Wireshark
* Firefox Web Browser
* Terminal (Ping command)
---
## 4. Methodology
The project was carried out by capturing live network packets while performing normal internet activities such as browsing websites and sending ping requests. The captured packets were then filtered and analyzed using Wireshark display filters.

---

## 5. Network Traffic Capture

Wireshark was opened in Kali Linux and the active network interface was selected. Live packet capture was started before generating any traffic to ensure all packets were recorded.

---

## 6. HTTP Traffic Analysis

To analyze HTTP traffic, an HTTP-only website (**[http://neverssl.com](http://neverssl.com)**) was accessed using Firefox. The display filter `http` was applied in Wireshark.

### Observation:

* HTTP packets were visible in plain text
* GET requests and server responses could be read
* Communication was unencrypted

This shows that HTTP traffic is insecure and can be easily intercepted by attackers.

**Screenshot Space:**
<img width="1920" height="1012" alt="image" src="https://github.com/user-attachments/assets/8ac6edeb-5f82-4849-8589-b89d60e56c36" />

---
## 7. HTTPS (TLS) Traffic Analysis

HTTPS traffic was analyzed by visiting secure websites such as Google and YouTube. The display filter `tls` was applied in Wireshark.

### Observation:

* Packets were encrypted
* No readable content was visible
* Secure TLS communication was observed

This confirms that HTTPS protects user data using encryption.

**Screenshot Space:**
<img width="1920" height="1012" alt="image" src="https://github.com/user-attachments/assets/ca249a4a-f4a2-49e0-950e-f82cfded0c4f" />

---

## 8. DNS Traffic Analysis

DNS traffic was analyzed using the `dns` display filter.

### Observation:

* DNS query and response packets were visible
* Domain names were resolved to IP addresses

DNS traffic helps in understanding how websites are located on the internet.

**Screenshot Space:**
<img width="1920" height="1012" alt="image" src="https://github.com/user-attachments/assets/5afd1610-e3bd-483a-93a8-779106346662" />

---

## 9. ICMP Traffic Analysis

ICMP traffic was generated using the `ping google.com` command in the terminal. The `icmp` filter was applied in Wireshark.

### Observation:

* ICMP Echo Request and Echo Reply packets were captured
* ICMP is mainly used for connectivity testing

Excessive ICMP traffic may indicate scanning or reconnaissance activity.

**Screenshot Space:**
<img width="1920" height="1012" alt="image" src="https://github.com/user-attachments/assets/67fbf042-a044-42a4-aad2-e3dc779d4777" />

---

## 10. Suspicious Traffic Observation

During analysis, repeated ICMP packets and multiple requests to the same destination were observed. Such patterns can sometimes indicate suspicious behavior like network scanning.

**Screenshot Space:**
<img width="1920" height="1012" alt="image" src="https://github.com/user-attachments/assets/a6c2b798-7ed5-47f2-ab81-4acc3b67d2d7" />


## 11. Results and Findings

* HTTP traffic is unencrypted and insecure
* HTTPS traffic is encrypted and secure
* DNS traffic reveals domain name resolution
* ICMP traffic is useful for network diagnostics
---
## 12. Conclusion

This project provided hands-on experience in capturing and analyzing real-time network traffic using Wireshark. It improved understanding of network protocols and highlighted the importance of secure communication. The project also demonstrated how attackers can analyze unencrypted traffic, emphasizing the need for HTTPS and proper network security practices.

---

**Author:** 
Bhairavi shewale 
bsc(Cyber & digital science )

