# Maven-Release仓库

UBSI欢迎您的到来！如果您有任何关于UBSI的问题，可以使用 [Issues功能](https://github.com/ubsi-home/release/issues) 与我们进行交流，或者发送email到ubsi@rewin.com.cn，我们会及时给您回复。

如果需要使用UBSI的发行包，请在maven的settings.xml中增加本仓库的引用：
```
<profiles>
  ......

  <profile>
    <id>github</id>
    <repositories>
      <repository>
        <id>github</id>
        <url>https://maven.pkg.github.com/ubsi-home/release</url>
      </repository>
    </repositories>
  </profile>
</profiles>
```
感谢您的关注!
