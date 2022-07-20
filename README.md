# Text Encoding (2021/22)
Project contained in this <i>repository</i> was created for <b>Text Encoding</b> exam, coordinated by <i>Angelo Mario Del Grosso</i>, from students of Digital Humanities:
- <i>Corrado Baccheschi</i> (mat. 599107)

- <i>Vincenzo Sammartino</i> (mat. 599203)  (repository : https://github.com/ilsamaritano/CodificaDiTesti)

The project was validated with Xerces by follow command:

## Xerces validation

```shell
$ java -cp "Xerces-J-bin.2.12.1/xerces-2_12_1/xml-apis.jar;Xerces-J-bin.2.12.1/xerces-2_12_1/xercesImpl.jar;Xerces-J-bin.2.12.1/xerces-2_12_1/xercesSamples.jar" dom.Counter prolusioni.xml
```

XML and XSL files were transformed with Saxon-HE 10.3 to HTML file "<i>prolusioni.html</i>" by follow command:

## XSL transform

```shell
$ java -jar ./SaxonHE10-3J/saxon-he-10.3.jar -s:prolusioni.xml -xsl:stile.xsl -o:prolusioni.html
```
Result:
```
prolusioni.xml: 144;31;1 ms (1142 elems, 3177 attrs, 8633 spaces, 39644 chars)
```

## Preview

https://hydrerscript.altervista.org/codifica/prolusioni.html
