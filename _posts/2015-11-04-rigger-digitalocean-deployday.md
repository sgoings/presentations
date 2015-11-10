---
title: "Ramping up with Rigger: Deploying Deis on DigitalOcean"
layout: reveal
author: Seth Goings
---
<img src="/presentations/assets/img/DeisLogo.png" class="stretched" style="border:none;background:none;box-shadow:0 0 0"/>

Seth Goings / [@sethgoings](http://twitter.com/sethgoings)

---

<img src="/presentations/assets/img/people/sgoings/sgoings-backhoe.jpg" class="stretched" style="border:none;background:none;"/>

---

## Deis Provisioning
## (yesteryear)

* ... circa Summer 2015
* [Creating Infrastructure](http://docs.deis.io/en/v1.9.1/installing_deis/digitalocean/)
* [Installing Deis](http://docs.deis.io/en/v1.9.1/installing_deis/install-platform/)

---

<iframe data-autoplay class="stretch" src="https://www.youtube.com/embed/d9OzjhAS-5Q" frameborder="0" allowfullscreen></iframe>

---

## Deis Provisioning
## ("to-day-morrow")

---

## Something better ...

---

## Wait for it ...

---

## [Rigger](https://github.com/deis/rigger)

---

## Step 1: Get Rigger

```
$ git clone https://github.com/deis/rigger.git
```

---

## Step 2: ???

```
$ rigger configure
```

---

## Step 3: Profit!

```
$ rigger provision
```

---

## Step 4 - Playtime!

```
git clone https://github.com/deis/example-nodejs-express.git
cd example-nodejs-express
source ~/.rigger/vars
deis auth:register "http://deis.${DEIS_TEST_DOMAIN}"
deis keys:add
deis apps:create
git push deis master
```

---

[Ramping Up With Rigger - Deploying Deis on DigitalOcean](https://www.digitalocean.com/community/tutorials/ramping-up-with-rigger-deploying-deis-on-digitalocean)

---

## Thanks

* [twitter.com/sethgoings](http://twitter.com/sethgoings)
* [github.com/sethgoings](http://github.com/sethgoings)
* sgoings@deis.com

---

![DeisBackground](/presentations/assets/img/DeisBackground.jpg)
