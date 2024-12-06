**Incident report analysis**

**Instructions**

As you continue through this course, you may use this template to record your findings after completing an activity or to take notes on what you've learned about a specific tool or concept. You can also use this chart as a way to practice applying the NIST framework to different situations you encounter.

| Summary | Today there were multiple reports of our clients not being able to request services from our servers. Eventually, the whole network was compromised and stopped responding altogether. We believe this to be some sort of Denial of Service attack which involves flooding our network with a large volume of spam. There have been noticeably large amounts of network traffic just prior to the network failure.   |  |  |
| :---- | :---- | ----- | ----- |
| Identify | The incident management team audited the network activities with tcpdump and have discovered there have been large amounts of Internet control message protocol error messages sent to the network through our firewall from various sources. This is an indication of a DDos attack.  |  |  |
| Protect | The security team has reconfigured the firewall to limit the amount of ICMP error messages to the network. The source IP addresses of incoming packets are checked for IP spoofing to reduce authorized access by malicious actors. |  |  |
| Detect | IDP/IPS system to detect and filter out anomalies and suspicious activities.  |  |  |
| Respond | Security team blocked incoming ICMP messages and stopped all non-critical network services. |  |  |
| Recover | Critical network services were restored to their original state. Any requests during the 2 hour down period are voided and customers are encouraged to send new requests. |  |  |

---

| Reflections/Notes: Firewall needs to be checked regularly to ensure it’s up to date SIEM can be used to aggregate all the known info of incident into single pane of glass |
| :---- |

