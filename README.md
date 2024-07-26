# es7笔记
spring官网文档： https://docs.spring.io/spring-data/elasticsearch/docs/4.2.5/reference/html/#preface

## 使用方式详见测试用例

- [RawCrudTest](src/test/java/com/my/es/demo/test/RawCrudTest.java) 使用RestClient, 最灵活，最不方便

- [BasicCrudTest](src/test/java/com/my/es/demo/test/BasicCrudTest.java) 使用ElasticsearchRestTemplate，最方便，最不灵活

- [ComplexQueryTest.java](src/test/java/com/my/es/demo/test/ComplexQueryTest.java) 使用RestHighLevelClient，折中

> 实际项目开发中，以RestHighLevelClient为主，以ElasticsearchRestTemplate为辅, RestClient一般用于用户在页面上自主组装查询条件，如低代码
