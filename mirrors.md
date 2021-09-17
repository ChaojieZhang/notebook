# mirrors

## npm

- npm

  ```
  npm config set registry https://registry.npm.taobao.org
  ```

- yarn

  ```
  yarn config set registry https://registry.npm.taobao.org
  ```

## go

### proxy

- Goproxy.cn: https://goproxy.cn
- 阿里云 Go Module: https://mirrors.aliyun.com/goproxy/

### setting

via environment variable

```
export GOPROXY=https://goproxy.cn
```

via go command

```
go env -w GOPROXY=https://goproxy.cn,direct
```

## homebrew

https://mirrors.tuna.tsinghua.edu.cn/help/homebrew/

## maven

```xml
<mirrors>
    <mirror>
      <id>alimaven</id>
      <name>aliyun maven</name>
      <url>http://maven.aliyun.com/nexus/content/groups/public/</url>
      <mirrorOf>central</mirrorOf>
    </mirror>
  </mirrors>
```

hard replace setting script

```sh
cat > ~/.m2/settings.xml <<EOL
<settings xmlns="http://maven.apache.org/SETTINGS/1.0.0" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="http://maven.apache.org/SETTINGS/1.0.0 https://maven.apache.org/xsd/settings-1.0.0.xsd">
    <mirrors>
        <mirror>
            <id>aliyunmaven</id>
            <mirrorOf>*</mirrorOf>
            <name>阿里云公共仓库</name>
            <url>https://maven.aliyun.com/repository/public</url>
        </mirror>
    </mirrors>
</settings>
EOL
```

## docker

## apt
