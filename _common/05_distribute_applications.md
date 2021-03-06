---
layout: default 
title: 5. Distribute the certificate to applications
collection: common
permalink: common/distribute-apps/
---

{% include alert-info.html content="<strong>We're calling for all solutions!</strong> If you'd like to share your agency's playbook on how to distribute a trusted root CA certificate to an application trust store, create an <a href=\"https://github.com/GSA/fpki-guides/issues/new\" target=\"_blank\">issue on GitHub</a> or email us at fpkirootupdate@gsa.gov." %}

Many, but not all, software applications leverage the underlying operating system [trust store]({{site.baseurl}}/truststores/) to verify whether a certificate should be trusted. 

Collaborate across agency teams to identify applications that rely on custom trust stores to ensure distribution of the Federal Common Policy CA (FCPCA) G2 certificate.

**Example applications with custom trust stores:**
- Java and all Java-based applications (for example, Apache Tomcat)
- Mozilla products (for example, Firefox or Thunderbird)
- OpenSSL-based applications (for example, Apache HTTP Server or Nginx)


{% include alert-warning.html content="<strong>Important!</strong> Depending on how these applications are configured, it's likely you'll also need to distribute the <a href=\"../certificates\">intermediate CA certificates</a> issued by the FCPCA G2." %}

<br>

Optionally, [distribute the CA certificates issued by the FCPCA G2]({{site.baseurl}}/common/certificates/).
