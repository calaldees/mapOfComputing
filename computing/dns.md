DNS
===

* [DNS Explained - How Domain Names Get Resolved](https://www.bhusalmanish.com.np/blog/posts/dns-explained.html)
* [wirewiki.com](https://www.wirewiki.com/) Explore internet infrastructure

```bash
dig
whois
```

* [The European public DNS that makes your Internet safer.](https://www.dns0.eu/)
    * [HN Comments](https://news.ycombinator.com/item?id=44267091)

* [ICANN Update: Launching RDAP; Sunsetting WHOIS](https://www.icann.org/en/announcements/details/icann-update-launching-rdap-sunsetting-whois-27-01-2025-en)

> It's always DNS
Kind of meme joke, but with big systems, it often is.
Global: one
> We're making too many DNS requests in the stack, while our DNS servers are fine, it looks like we're taxing the AWS DNS resolvers in our VPC.  Because of how the DNS resolve.conf is setup in our pods, we end up searching based on domain search paths making 5 DNS requests per resolution.  This change reduces the load in 2 ways:
> Fully qualified xxx endpoint: The full qualified endpoint is greater than the number of dots ndots so this turns off DNS searching.Reduces the number of dots that will be used in DNS 'searching', xxx.xxx has one dot so will result in DNS searching, but www.google.com has 2 dots so will be treated as a fully qualified domain and not search.
```yaml
xxx_ENDPOINT: http://xxx.xxx.svc.cluster.local
```
```yaml
      dnsConfig:
        options:
          - name: ndots
            value: "1"
```

Both of these changes combine to only have a single request per DNS resolve.
* [The secret life of DNS packets: investigating complex networks](https://stripe.com/blog/secret-life-of-dns)
    * Case study of debugging spikes in reverse dns requests at stripe.com
    * Cool they found it rate limiting to 1024 requests a second which was causing more panic and retries
    * Use of `tcpdump` (more needed)
* [Please do not put IP addresses into DNS MX records](https://blog.hboeck.de/archives/904-Please-do-not-put-IP-addresses-into-DNS-MX-records.html)
    * DNS server request / lookup? 

* [Let's hand write DNS messages](https://routley.io/posts/hand-writing-dns-messages/)
    * with python - send binary [[udp]]
* [how can i decipher dns messages?](https://stackoverflow.com/questions/13372860/how-can-i-decipher-dns-messages)
* [rfc1035](https://datatracker.ietf.org/doc/html/rfc1035)

* [RFC 9076: DNS Privacy Considerations](https://www.rfc-editor.org/rfc/rfc9076.html) [[privacy]]

* [Shortest URLs on the Internet](https://jameswillia.ms/posts/shortest-urls.html)
    * http://ai (it works!)

* Mullvad VPN: [Shutting down our unencrypted public DNS service](https://mullvad.net/en/blog/2022/12/13/shutting-down-our-unencrypted-public-dns-service/) Dec 2022
    * non encrypted DNS is bad

Security
--------

* [dnsteal](https://github.com/m57/dnsteal)
    * > a fake DNS server that allows you to stealthily extract files from a victim machine through DNS requests
    * This is interesting because logging is normally done my monitoring TCP - most security firewalls let DNS traffic through


[udp]: udp.md "UDP"
[privacy]: privacy.md "Privacy"

