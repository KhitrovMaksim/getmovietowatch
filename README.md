# Get Movie To Watch
**getmovietowatch.com** - service will help you choose a movie to watch.

## Structure
```
repository
├─ clients
│   └─ site - getmovietowatch.com
├─ servers
│   ├─ api - api.getmovietowatch.com
│   └─ database - getmovietowatch.com
├─ README.md
├─ .editorconfig
└─ .gitignre
```

----

## Clients
1. Site:
- **Entry point**: getmovietowatch.com/
- **Stack**: React, TypeScript, Vite, REST API, JWT

## Servers
1. Api
- **Entry point**: api.getmovietowatch.com
- **Stack**: NestJS, REST API
- **Versioning**: header "X-GetMovieToWatch-Api-Version:2023-09-01"
2. Databases
 - **Entry point**: getmovietowatch.com
 - **Stack**: Postgres, pgAdmin

----

## DevOps
**Stack**: Docker, Docker-compose, Ubuntu, PostgreSQL
### Infrastructure
#### Production servers
- server 1:
  - for: containers with clients and servers
  - configuration: CPU 1*2.8 RAM 2GB SSD 15GB
  - os: Ubuntu 22.04.2 LTS

#### CI/CD pipelines
1. Production:
   - **Hook**: GitHub Actions on release branch manually
   - **Stages**:
     - build image
     - push to AWS ECR
     - run container
     - tests

----

## Git flow

```shell
git commit -m "commit_message resolve #337"
```

----

## Quick start
Setup environment
1. Clone repo
```shell
git clone https://github.com/KhitrovMaksim/getmovietowatch.git
cd getmovietowatch
git config core.autocrlf input
```
2. Setup IDE
 - Open cloned repo in IDE
 - Enable EditorConfig support
 - End of line - lf
