---
layout: post
title: "Linux cut Command"
date: 2012-10-11 09:03
comments: true
categories: [linux, ubuntu, cli]
---

The `cut` command can be used to take vertical slices of lines in a
file. Say you have a file of currencies:

    GYD 328	Guyanese dollar
    HKD 344	Hong Kong dollar
    HNL 340	Honduran lempira
    HRK 191	Croatian kuna

And you only need currency code and numeric code. The Linux `cut` command will be quite handy here:

    cut -f 1,2 currencies

This will produce:

    GYD 328
    HKD 344
    HNL 340
    HRK 191

The above command takes field 1 and 2 where "field" delimiter is
TAB. You can change delimiter by specifying `-d <delimiter>`.

The `--output-delimiter` can be used to seperate fields by comma.

    cut -f 1,2 --output-delimiter=', ' currencies

This will procude:

    GYD, 328
    HKD, 344
    HNL, 340
    HRK, 191
