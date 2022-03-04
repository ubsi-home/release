# Maven-Release仓库

UBSI欢迎您的到来！如果您有任何关于UBSI的问题，可以使用 [Issues功能](https://github.com/ubsi-home/release/issues) 与我们进行交流，或者发送email到ubsi@rewin.com.cn，我们会及时给您回复。

如果需要使用UBSI的发行包，请在maven的settings.xml中增加本仓库的引用：
```
<servers>
  ......

  <server>
    <id>github</id>
      <username>{your-github-account}</username>
      <password>{your-github-Personal_access_tokens}</password>
      <!-- Personal access tokens需要具备的权限：public_repo | read:packages -->
      <!-- 可以在github.com的个人Settings -> Developer settings -> Personal access tokens页面中创建PAT -->
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
