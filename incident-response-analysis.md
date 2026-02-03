# Incident Response Analysis Using NIST CSF

Summary

A multimedia company experienced a denial-of-service (DoS) attack that disrupted internal network services for approximately two hours. The attack was caused by a flood of ICMP packets entering the network through an improperly configured firewall. During the incident, internal users were unable to access network resources until mitigation steps were implemented.

The incident management team responded by blocking ICMP traffic, taking non-critical services offline, and restoring critical services. Following containment, the cybersecurity team conducted an investigation and implemented additional controls to prevent future incidents.

## Identify

The cybersecurity team identified the following during the investigation:

- The attack was an ICMP flood resulting in a denial-of-service (DoS).
- The organization’s firewall lacked rules to limit or filter incoming ICMP traffic.
- Network services were overwhelmed and became unavailable to internal users.
- The attack originated from an external source exploiting the unconfigured firewall.

Affected assets included internal network services and firewall infrastructure.

---

## Protect

To improve protection against future incidents, the following safeguards were implemented:

- Firewall rules were updated to rate-limit incoming ICMP packets.
- Source IP address verification was enabled to detect spoofed IP addresses.
- Network security policies were reviewed and updated to restrict unnecessary traffic.

These measures help reduce the attack surface and prevent unauthorized traffic from overwhelming network resources.

---

## Detect

To improve detection capabilities, the organization implemented:

- Network monitoring software to identify abnormal traffic patterns.
- An IDS/IPS system to detect and filter suspicious ICMP traffic.
- Enhanced firewall logging to provide visibility into inbound network traffic.

These tools enable faster identification of denial-of-service attacks and other network anomalies.

---

## Respond

The response plan for future incidents includes:

- Immediately blocking malicious traffic at the firewall.
- Isolating affected network segments if necessary.
- Temporarily disabling non-essential services to preserve critical operations.
- Notifying internal stakeholders and documenting incident details.

Post-incident reviews will be conducted to identify response improvements.

---

## Recover

Recovery efforts focused on restoring normal network operations and improving resilience:

- Critical network services were restored after traffic filtering was applied.
- Non-critical services were brought back online after system stability was confirmed.
- Recovery procedures were reviewed and updated to improve response time in future incidents.

---

## Conclusion

Applying the NIST Cybersecurity Framework allowed the organization to systematically analyze the DoS attack and strengthen its security posture. Improvements in firewall configuration, monitoring, and response planning reduce the likelihood and impact of similar attacks in the future.
