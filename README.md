pretty
======

A tool for common use of convert structed (xml, json etc.) data to unix text format.

Install
=======

Usage
=====

```sh
pretty test.xml | tgrep '$1~/US/ $2~/LA/'
curl http://test.com/test.json | pretty | grep ^name
```
