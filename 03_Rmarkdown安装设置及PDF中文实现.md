# Rmarkdown安装设置及PDF中文实现

## 安装R和Rstudio

关于R-studio的一些设置，一般会在toools->global options->Packages中将CRAN 的默认mirror地址改为中国的镜像，这样在安装包的时候速度可以更快些。

## 安装 rmarkdown 包
```r
install.packages("rmarkdown")
```

## 安装 tinytex 包

```r
devtools::install_github('yihui/tinytex')
tinytex::install_tinytex()
```

步骤较慢，过程中若出现无法连接可提前打开相应网页并反复重试

Tinytex文档：https://yihui.org/tinytex/cn/

## 安装rticles包，调用中文模板

```r
install.packages("rticles")
```

安装成功之后，可以新建一个Rmarkdown文件。点击New->file->R markdown,其中有了一个From Template，如果没有看到，检查rticles包是否安装成功，之后请载入该包(library(rticles))。

成功新建之后可以看到已经有一个模板，我们可以点击knit按钮，或者使用ctrl + shift + k的快捷键，稍等片刻会出现中文PDF。

注：第一次运行由于需要进行相关安装文件的下载安装会比较慢。
