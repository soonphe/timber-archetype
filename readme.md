# timber——archetype

## 项目介绍（Project Introduction）
archetype模板项目，快速生成api,servier,web等项目/模块

### 业务功能模块（functional module）
- timber-api-template ：api模块生成
- timber-service-template：service模块生成
- timber-web-template

### 快速开始
```
下载项目、本地打包
mvn clean install

爬取项目骨架
mvn archetype:crawl
```

#### 命令示例
api 工程模板执行
```
mvn archetype:generate  -DgroupId=com.soonphe.timber -DartifactId=test-api -Dversion=1.0.0-SNAPSHOT -Dpackage=com.soonphe.timber.api -DarchetypeArtifactId=timber-api-template -DarchetypeGroupId=com.soonphe.timber -DarchetypeVersion=1.0.0-SNAPSHOT -DdataId=test-api
```

service 工程模板执行
```
mvn archetype:generate  -DgroupId=com.soonphe.timber -DartifactId=test-biz -Dversion=1.0.0-SNAPSHOT -Dpackage=com.soonphe.timber.service -DarchetypeArtifactId=timber-service-template -DarchetypeGroupId=com.soonphe.timber -DarchetypeVersion=1.0.0-SNAPSHOT -DdataId=test-biz
```

#### 变量释义
* groupId    | 组名(一般情况下不要改)
* artifactId | 工程名字
* package    | 包名 com.soonphe.timber.业务名
* dataId     | nacos 上dataId                                        
