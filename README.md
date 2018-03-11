# SICP

## 安装

	可参考 [MIT-Scheme 安装](https://segmentfault.com/a/1190000007556974) 一文，介绍的非常详细，此处简略说明主要步骤

1. 去 [官网](https://www.gnu.org/software/mit-scheme/) 下载，或者 [点此下载](http://ftp.gnu.org/gnu/mit-scheme/stable.pkg/9.2/mit-scheme-9.2-x86-64.dmg)
2. 设置软链接
```
sudo ln -s /Applications/MIT\:GNU\ Scheme.app/Contents/Resources/mit-scheme /usr/local/bin/scheme
```
3. 设置环境变量
```
echo "export MITSCHEME_LIBRARY_PATH=\"/Applications/MIT\:GNU\ Scheme.app/Contents/Resources\"" >> ~/.profile

echo "export MIT_SCHEME_EXE=\"/usr/local/scheme\"" >> ~/.profile
```
4. reload bash profile
```
source ~/.profile
```
5. 检测设置是否生效

```
scheme
```

![](https://gw.alicdn.com/tfs/TB1KihydntYBeNjy1XdXXXXyVXa-1114-442.png)

## 基本用法

1. 编写 `test.scm` 文件
```
(define (sum a b) (+ a b))
```
2. 输入 `scheme` 命令进入环境
3. 输入`(load "test.scm")`
```
1 ]=> (load "test.scm")

;Loading "test.scm"... done
;Value: sum
```
4. 然后就可以使用 test.scm 中的函数了，例如 
```
1 ]=> (sum 8 3)

;Value: 11
```
5. 常用命令

		1. `ctrl+z`
		2. `ctrl+g`


## 参考资料

1. [习题参考答案](http://sicp.readthedocs.io/en/latest/)
2. [SICP读书笔记](https://github.com/jiacai2050/sicp)
3. [北大程序设计技术和方法-教学主页](http://www.math.pku.edu.cn/teachers/qiuzy/progtech/)
4. [MIT-Scheme入门教程](https://www.w3cschool.cn/yast_cn/6lxnmozt.html)

## Timeline

* 2018-03-10 开启SICP之旅
