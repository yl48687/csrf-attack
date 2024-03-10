# CSRF Attack
The project utilizes the Cross-Site Request Forgery (CSRF) Lab provided by SEEDLAB 2.0 as a foundational platform for hands-on exploration and experimentation in the domain of web security. The Cross-Site Request Forgery (CSRF) attack is a prevalent threat that exploits the trust relationship between a victim user and a trusted site, wherein a malicious site manipulates the victim's session to perform unauthorized actions on the trusted site.

The lab focuses on conducting CSRF attacks on a social networking web application called Elgg, which serves as an illustrative example. Within the SEEDLAB-provided virtual machine (VM), Elgg has been pre-installed, offering an ideal environment for experimentation. Notably, countermeasures against CSRF within Elgg have been deactivated to allow for comprehensive exploration during the lab session.

Key topics covered in this lab include an introduction to the CSRF attack, the implementation of countermeasures such as secret tokens and Same-site cookies, an examination of HTTP GET and POST requests, and the role of JavaScript and Ajax in facilitating CSRF exploits.

## Report
The detailed project report, including the methodology, findings, and analysis of CSRF attack techniques and countermeasures, can be accessed in the attached `Report.pdf`.

## Additional

### Original Lab Instructions
The original lab instructions outlining the objectives, tasks, and guidelines for the CSRF Attack Lab can be accessed [here](https://seedsecuritylabs.org/Labs_20.04/Web/Web_CSRF_Elgg/).

### Modified Files
The modified files according to lab instructions are as follows:
- `addfriend.html`
─ `editprofile.html`

The original (non-modified) files can be found in the `Labsetup` directory within this repository.

## File Structure and Content
```
csrf-attack/
├── addfriend.html
├── editprofile.html
├── Labsetup/
│   ├── attacker
│   │   ├── addfriend.html
│   │   ├── editprofile.html
│   │   ├── index.html
│   │   └── testing.html
│   ├── docker-compose.yml
│   ├── image_attacker/
│   │   ├── apache_attacker.conf
│   │   ├── Dockerfile
│   │   └── server_name.conf
│   ├── image_mysql/
│   │   ├── Dockerfile
│   │   └── elgg.sql
│   └── image_www/
│       ├── apache_defense.conf
│       ├── apache_elgg.conf
│       ├── defense/
│       │   ├── index.php
│       │   ├── showcookies.php
│       │   └── testing.html
│       ├── Dockerfile
│       └── elgg/
│           ├── ajax.js
│           ├── Csrf.php
│           └── settings.php
├── README.md
└── Report.pdf
```