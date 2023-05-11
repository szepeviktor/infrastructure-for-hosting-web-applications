# Special infrastructure for web applications

[![hu](https://img.shields.io/badge/nyelv-magyar%20%F0%9F%87%AD%F0%9F%87%BA-white)](README.hu.md)
[![en](https://img.shields.io/badge/lang-english%20%F0%9F%87%AC%F0%9F%87%A7-white)](README.md)
[![theories](https://img.shields.io/badge/more-theories-purple)](https://github.com/stars/szepeviktor/lists/theory)

This document is the result of several hundreds of real-life incidents.
`#SaaS`

My policy on providing services is to **use specialized service providers**,
not popular ones, never free ones.

## WWW

🪨 The World Wide Web is part of the Internet,
so we need to connect to the Internet and provide web services.

## Infrastructure

- Domain registrar
- DNS provider
- Server provider
- SSL certificate vendor
- CDN provider
- Transactional email provider
- Storage provider for backup

## Enterprise ready server provider

"Cloud" really means virtualization **and** server clusters.
Many so-called cloud providers only virtualize a single physical server.

1. Software defined **and** redundant network
2. Software defined **and** redundant storage
3. Software defined **and** redundant servers
    (CPU+memory) 👈🏻 this is very-very hard
4. Thin, thus performant virtualization layer

## OS, middleware, runtime

1. Build on Debian GNU/Linux
2. Know each software on your server; uninstall all unused
3. Keep every file on your server under control (e.g. packages, git)
4. Monitor the kernel, the filesystem and every server software
    with functional tests, not just "pings"

### Middleware

- Apache httpd
- PHP-FPM (FastCGI Process Manager)
- Redis in-memory cache
- MariaDB database

## The Web Application

Write as little code as it is possible.
Build on well-tested packages and **specialized** providers.

- Integrated customer relations
- Fonts
- Videos
- Maps
- HTML widgets
- Advertisement
- Visitor tracking
- Payment gateway
- Email address verification
- SMS gateway
- Authentication
- Error tracking

Run production environments without humans.
Every problem should be solvable with CI
and anonymized staging environments.

💡 Recognize your tech debt when you are manually working
on a production environment.

Only 1 _Tech Debt Day_ per month can tip the scales from stress to joy.

## Cooperating with providers, software authors

Your application depends on others!

### Analyze your service providers

- Target audience
- Specialized provider vs. populist provider (quality vs. quantity)
- Funds
- Talk to the CEO and employees
- Discovery expertise by reading their blog, asking for a demo
- Attitude and transparency
- Usability
- Infrastructure
- Service providers
- Integrations and API-s
- Price-value ratio

### Know the software authors you depend on

- Attitude
- Response to bug reports
- Openness to contributors
- Coverage
- Release frequency
- QA tools in CI
