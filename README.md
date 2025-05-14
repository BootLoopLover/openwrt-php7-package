 

Compile PHP7 modules
====================

Follow the cross compile tutorial on the Omega site
https://wiki.onion.io/Tutorials/Cross-Compile

In the step 3, add the PHP7 repo

```
echo "src-git php7 https://github.com/BootLoopLover/openwrt-php7-package.git" >> feeds.conf.default
```

```
scripts/feeds update -a
scripts/feeds install -a
```
