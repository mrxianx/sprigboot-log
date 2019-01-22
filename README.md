# sprigboot-log
切面收集日志，采用spring boot2.0 开发切面服务，打成jar包，供外部服务引用，收集接口日志信息

imccp-cloud-log为日志服务
jar-test 为测试服务


1.特别注意pom.xml中，打成jar，不能使用默认spring boot打包方式，要采用maven打包方式，详见imccp-cloud-log中pom.xml


2.外部服务引用时，需要在启动类上添加扫描，@ComponentScan({"com.inphase.imccp","com.example.test.jartest"})，逗号之前为jar包根路径，后面位项目根路径