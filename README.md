# Maven-Release仓库

UBSI欢迎您的到来！release仓库是用来托管UBSI的核心JAR包以及可部署的基础微服务JAR包，这些JAR包可以通过maven进行引用，各个包的详情请查看：https://github.com/orgs/ubsi-home/packages

在maven的settings.xml中增加本仓库的引用：
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
如果您有任何关于UBSI的问题，可以使用 [Issues功能](https://github.com/ubsi-home/release/issues) 与我们进行交流，或者发送email到ubsi@rewin.com.cn，我们会及时给您回复。
谢谢您的关注! 
