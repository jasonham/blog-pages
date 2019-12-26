---
title: 如何在travis ci自动部署时设置自定义域名
date: 2019-12-16 00:26:50
update: 2019-12-16 00:26:50

tags:
 - travis ci
 - github pages
category:
 - [技术, travis ci, github pages]
---

在Travis CI部署Github pages时，默认是不会生成自定义域名的，每次都需要去Github的setting里重新设置一下。如果需要在部署时自动配置好自定义域名，可以在 .travis.yml的deploy内添加

``` yml .travis.yml
...
deploy:
  fqdn: [你的域名]
...
```