# Server-Setup

- IP Address: 3.81.228.240/
- URL: http://3.81.228.240/launch_manifest/

- Summary of software installed:
    - postgres
    - python-sqlalchemy
    - python-pip
    - apache
    - libapache2-mod-wsgi
    - git

- Summary of configuration made:
    - Firewall:
        - allowed connection for:
            - SSH on port 2200
            - HTTP on port 80
            - NTP on port 123
        - denied connection for SSH on **deafult** port 22
    - User management:
        - created users `grader`
        - disabled login for `root`
        - required users to authenticate using `RSA` keys
    - set up `postgres` to listen on default port `5432`
    - set up the web server to listen on port `80`

- third party resources used:
    - the `do-release-upgrade` command from aws LightSail
