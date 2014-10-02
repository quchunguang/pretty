pretty
======

**Pretty** is a unix-style text format designed for display structed data.
**Pretty** is a tool for common use of convert structed (xml, json etc.) data to pretty format.

But, why we need a new text format? we have dsv, rfc 822, Cookie-Jar, Record-Jar, xml, ini, ...

* Original unix-style format can perfectly store and process (via grep/awk/sed/wc/sort/cut... toolkit) record data, but not structed data, like tree and graph.
* Xml... can clearly display tree-like structed data, but not very efficiency.
* Xml... can NOT use grep... toolkit. pyxie(a xml switch format) make a not successful try about this issue. 
* I can not find a good text format for clearly display graph-like structed data.
* There is already many software (especially on linux) generate structed data can be seen as **pretty**.

Install
=======

Make sure you have installed golang and export $GOPATH/bin to $PATH.

```sh
go get github.com/quchunguang/pretty
```

Usage
=====

```sh
pretty test.xml | tgrep '$1~/US/ $2~/LA/'
curl http://test.com/test.json | pretty | grep ^name
```

