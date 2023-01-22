# Specialized instrastructure for web applications

This document is the result of several hundreds of real-life incidents.
`#SaaS`

My policy on providing services is to **use specialized service providers**,
not popular ones, never free ones.

## WWW

🪨 The World Wide Web is part the Internet,
so we need to connect to the Internet and provide web services.

## Infrastructure

- Domain registrar
- DNS provider
- Server provider
- SSL certificate vendor
- CDN provider
- Transactional email provider
- Storage provider for backup

## Premium server provider

"Cloud" really means virtualization **and** server clusters.
Many so-called cloud providers only virtualize a single server.

1. Software defined **and** redundant network
2. Software defined **and** redundant storage
3. Software defined **and** redundant servers
    (CPU+memory) 👈🏻 this is very-very hard
4. Thin thus performant virtualization layer

## OS, middleware, runtime

1. Build on Debian
2. Know each software on your server, uninstall all unused
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
and anonimized staging environments.

💡 Recognize your tech debt when you are manually working
on a production environment.

Only 1 _Tech Debt Day_ per month can tip the scales from stress to joy.

## Cooperating with providers, software authors

Your application depends on others!

### Analyze your service providers

- Target audience
- Specialized provider vs. populist provider (quality vs. quantity)
- Funds
- Talk to CEO and employees
- Discovery expertise by reading their blog, asking for a demo
- Attitude and tranparency
- Usability
- Infrastructure
- Service providers
- Integrations and API-s
- Price-value ratio

### Know software authors you depend on

- Attitude
- Response to bug reports
- Amount of unit tests
- Release frequency
- Amount of QA tools in CI
