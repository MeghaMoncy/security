# OSG-SEC-2026-01-27 CRITICAL ROOT Framework Remote Code Execution Vulnerability (CVE-2026-24811, CVE-2026-24812)

Dear OSG Security Contacts,

Two critical vulnerabilities, CVE-2026-24811 and CVE-2026-24812, have been identified in the ROOT framework, specifically within its bundled (builtins) version of the zlib library. ROOT is an open-source data analysis framework developed at CERN. It is the foundational software for high-energy physics.

## IMPACTED VERSIONS:
All versions up to and including 6.36.00-rc1

## WHAT ARE THE VULNERABILITIES:
The flaws reside in inffast.c (pointer arithmetic error) and inftrees.c (buffer overflow). Because these handle the decompression of data, an attacker can exploit them by providing a maliciously crafted .root file or compressed data packet. The initial compromise grants the privileges of the service user. This is not a vulnerability that allows privilege escalation.

## WHAT YOU SHOULD DO:

Upgrade to Version 6.36.00 (Stable) and higher.

## REFERENCES 
[1] https://nvd.nist.gov/vuln/detail/CVE-2026-24811 
[2] https://nvd.nist.gov/vuln/detail/CVE-2026-24812 
[3] https://github.com/root-project/root/pull/18526 
[4] https://github.com/root-project/root/pull/18527 
[5] https://github.com/advisories/GHSA-fm67-x2fw-2g76 


Please contact the OSG security team at security@osg-htc.org if you have any questions or concerns.

OSG Security Team
