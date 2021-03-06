<h1 align="center">sfNamaste</h1>
<p align="center">
<img src="https://cdn0.iconfinder.com/data/icons/sports-android-l-lollipop-icon-pack/24/floating_guru-256.png" />
</p>

<p align="center">
    <img src="http://4.bp.blogspot.com/-8SkMq_RvLAk/UAQPXDdlETI/AAAAAAAAA7k/XlM-IcFMF2I/s1600/symfony-logo.png" width="128" height="128" alt="Symfony 4"></img>
    <img src="https://www.docker.com/sites/default/files/Whale%20Logo332_5.png" width="128" height="128" alt="Docker"></img>
    <img src="https://avatars1.githubusercontent.com/u/5780637?s=400&v=4" width="128" height="128" alt="lopezator/sfdocker"></img>
    <img src="https://blog.savoirfairelinux.com/fr-ca/wp-content/uploads/2017/10/VQLBJ0TR_200x200.png" width="128" height="128" alt="GraphQL"></img>
<p>

<h6 align="center">Symfony 4 application boilerplate ready to use with Docker</h6>

<h3 align="center">Features</h3>

<ul align="center">
    <li><a href="https://symfony.com">Symfony 4</a></li>
    <li><a href="https://www.docker.com/">Docker</a> & <a href="https://docs.docker.com/compose/">Docker compose</a> (Includes PostgreSQL and Redis)</li>
    <li><a href="https://github.com/lopezator/sfdocker">Lopezator's sfdocker</a> script</li>
    <li><a href="http://graphql.org/">GraphQL</a> support with <a href="https://github.com/overblog/GraphQLBundle">overblog's GraphQLBundle</a></li>
</ul>

## Prerequisites
- [Docker](https://www.docker.com/) and [Docker compose](https://docs.docker.com/compose/) installed

## Installation

- Clone repository:
```bash
$ git clone https://github.com/edertxodw/sfNamaste
```
- Configure sfdocker:
```bash
$ ./sfdocker config
```
> **Default configuration:**

> Container: php-fpm

> User: www-data
- Build:
```bash
$ ./sfdocker build
```
- Install dependencies:
```bash
$ ./sfdocker yarn install
```
- Create database tables:
```bash
$ ./sfdocker console doctrine:schema:update --force
```

## Tweets

**sfNamaste** comes with a CRUD example entity. You can write
yor own __tweets__ from the example page at `http://localhost:3000/tweets`

## GraphQL

Integrates [overblog/GraphQLBundle(v 0.10)](https://github.com/overblog/GraphQLBundle/tree/0.10)
so you can create a **GraphQL** based query API.