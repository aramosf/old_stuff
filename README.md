# old_stuff

Archive of small, old projects, consolidated into a single repository. Each one
used to live in its own repository; they are gathered here to keep them
available without scattering the profile.

| Project | Years | What it is |
| --- | --- | --- |
| [`oldexploits`](oldexploits/) | 2005 – 2006 | Advisories and exploits of the era: phpBB 2.0.15, Drupal SA-2005-002, Nokia OBEX DoS, Cerberus Helpdesk SQLi, LifeType SQLi. See its own [index](oldexploits/README.md) |
| [`sameips`](sameips/) | 2007 – 2014 | Shell script to find hosts sharing an IP / several IPs on the same system, driving `nmap` sweeps and `hping2` TCP timestamps. [Write-up](http://www.securitybydefault.com/2009/10/sistemas-con-varias-direcciones-ip.html) |
| [`eapmd5hcgen`](eapmd5hcgen/) | 2014 | Turns an EAP-MD5 challenge/response captured from a pcap into a hashcat-ready hash plus rule file (WPA2-Enterprise). Based on `eapmd5crack.py` by Mark Baggett & Tim Tomes. [Write-up](http://www.securitybydefault.com/2014/01/wpa2-enterprise-cracking-de-eap-md5.html) |
| [`redis-portscan`](redis-portscan/) | 2014 | Port-scans a host *through* an exposed Redis server, inferring open ports from the error strings returned by `MIGRATE`. |
| [`filmaffinity-glftpd`](filmaffinity-glftpd/) | 2014 – 2017 | Sorts a glftpd site by FilmAffinity rating (Spanish films), runs from cron outside the chroot; includes director sorting and a cleanup script. |
| [`Cookiesmap`](Cookiesmap/) | 2015 | Freemind mind-map of HTTP cookies (`.mm` source plus SVG/PNG/HTML/JPEG renders). |
| [`mycheatertwitterfriends`](mycheatertwitterfriends/) | 2016 | Checks which of the accounts you follow on Twitter are inflated with bot followers, via twitteraudit. |
| [`na-dsm`](na-dsm/) | 2017 | Downloads Netgear Arlo cloud recordings onto a Synology DSM NAS. |
| [`plex_tools`](plex_tools/) | 2025 | Plex library utilities: detect missing TV episodes against TheTVDB, export movie metadata to CSV, move low-rated films, rename files from metadata. |

## Notes

- These are archived as they were, in a single commit: the per-project commit
  history of the original repositories is not carried over. The dates in the
  table above come from the code and the advisories themselves.
- Most of it targets Python 2, Perl of the era or long-dead APIs (Twitter
  v1.1, old TheTVDB); expect to port before running anything.
- The security-related material here (`oldexploits`, `sameips`, `eapmd5hcgen`,
  `redis-portscan`) is old proof-of-concept research: use it only against
  systems you own or are explicitly authorized to test.

## Credits

A. Ramos `<aramosf@gmail.com>` — earlier work here is signed with the handles
and addresses of its time (`dab @ !dSR` / `dab@digitalsec.net`,
`aramosf@unsec.net`, `aramosf@514.es`), and several of these were published
alongside articles on securitybydefault.com. The only outside contribution is
noted in the [`oldexploits` index](oldexploits/README.md).
