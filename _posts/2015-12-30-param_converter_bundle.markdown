---
layout: post
title:  "First bundle - Parameter converter bundle"
date:   2015-12-30 10:00:00
categories: php,packagist
---

Well, this happened a little bit earlier, but now it's official. Our first bundle
is online and on packagist. Namely - [Parameter converter bundle](http://github.gendoria.pl/param-converter-bundle/).
It's first, but we hope not least. 

Why another bundle for parameter conversion, when we have FrameworkExtraBundle, 
you may ask? Well, this one is add-on for it. FrameworkExtraBundle is great, 
but has only two converters: doctrine and DateTime. And, while this may last
for most of you, we foud it lacking something. Especially the ability
to call **arbitrary** service and method instead of just Doctrine repository.

If you, like we, do not use standard Doctrine repositories and managers, this bundle
will allow you to utilize their methods to fetch objects. You may then 
use these objects - for example - in security annotation. As, well, we do :)

Another converter, which has been added today, is ArrayObject param converter.
This is useful, if you want to pass several IDs in URL and be able to inject them as an array.
And why this? To inject them to service parameter converter as an argument, of course :).
Or to do anything you want, it's your call.