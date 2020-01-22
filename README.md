# pdftk-dockerfile
pdftk で PDFを結合するためのDocker環境の作成

# 利用例

```
$ docker build -t pdftk .
# 共有しているフォルダのすべてのpdf拡張子ファイルをresult.pdfとして結合
$ docker run --rm -v `pwd`:/work -it pdftk  *.pdf cat output result.pdf
```

