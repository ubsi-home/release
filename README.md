# Maven-Release仓库

UBSI欢迎您的到来！如果您有任何关于UBSI的问题，可以使用 [Issues功能](https://github.com/ubsi-home/release/issues) 与我们进行交流，或者发送email到ubsi@rewin.com.cn，我们会及时给您回复。

如果需要使用UBSI的发行包，请在maven的settings.xml中增加本仓库的引用：
```
<servers>
  ......

  <server>
    <id>github</id>
      <username>ubsi-user</username>
      <password>ghp_YGaAugA3CnkIZO2O-$-D5L5x87ar32cUL2VhB3O</password>
      <!-- 实际使用时，请去掉password中间的"-$-" -->
  </server>
</servers>

<profiles>
  ......

  <profile>
    <id>dev</id>
    <repositories>
      ......
      
      <repository>
        <id>github</id>
        <url>https://maven.pkg.github.com/ubsi-home/release</url>
      </repository>
    </repositories>
  </profile>
</profiles>

<activeProfiles>
  <activeProfile>dev</activeProfile>
</activeProfiles>
```
感谢您的关注!
