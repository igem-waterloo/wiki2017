# CiGEM

This year, we worked with U of T to adapt their [igemwiki-api](https://www.npmjs.com/package/igemwiki-api) into a continuous integration server. This server allows teams to edit their wikis locally and on GitHub and automatically upload them to igem.org servers when changes are made. This allows iGEM teams to write cleaner code and saves them time uploading that code manually.

## Continuous Integration

Continuous integration (CI) refers to a continuous process of integrating code after it is written. It is a very common practice in software development because it removes the unnecessary hassle of uploading by hand. It also ensures that the main repository which stores the code represents exactly what is seen on the website. This prevents confusion as to who changed what and ensures that those changes will never be lost.

## NodeJS

NodeJS is a platform for building Javascript programs that can be run on any machine. It is a very popular tool for building web servers and was what U of T iGEM made their igemwiki-api with. We decided to build the CI server with it because it is very fast, familiar for many web developers and natively supported the igemwiki-api.

## Implementation

CiGEM is hosted on Google App Engine and supports two endpoints. The endpoint "/payload/setup" accepts a team name and GitHub repository URL and "clones" the code as well as adds the team to a registry. The endpoint "/payload" checks for a GitHub push header. If it finds one, it pulls the code from GitHub and pushes it live to iGEM's servers. The setup for the server is as easy as making a request to the setup handler and adding a WebHook on GitHub. The code for the server can be found on [our GitHub repository](https://github.com/igem-waterloo/cigem)
