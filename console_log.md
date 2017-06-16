
/*****************************************************************************
**                     Build the JAR - mvn package              ***
******************************************************************************/
```
{Sat 10 Jun 12:59} -  ~/code_p/gatling/micro-services/ecommerce-microservices/user-microservice   master  mvn package
[INFO] Scanning for projects...
[INFO]
[INFO] ------------------------------------------------------------------------
[INFO] Building user-microservice 0.0.1-SNAPSHOT
[INFO] ------------------------------------------------------------------------
[INFO]
[INFO] --- maven-resources-plugin:2.6:resources (default-resources) @ user-microservice ---
[INFO] Using 'UTF-8' encoding to copy filtered resources.
[INFO] Copying 1 resource
[INFO] Copying 1 resource
[INFO]
[INFO] --- maven-compiler-plugin:3.1:compile (default-compile) @ user-microservice ---
[INFO] Changes detected - recompiling the module!
[INFO] Compiling 3 source files to ~/code_p/gatling/micro-services/ecommerce-microservices/user-microservice/target/classes

....
```
```
Results :

Tests run: 1, Failures: 0, Errors: 0, Skipped: 0

[INFO]
[INFO] --- maven-jar-plugin:2.5:jar (default-jar) @ user-microservice ---
[INFO] Building jar: ~/code_p/gatling/micro-services/ecommerce-microservices/user-microservice/target/user-microservice-0.0.1-SNAPSHOT.jar
[INFO]
[INFO] --- spring-boot-maven-plugin:1.2.7.RELEASE:repackage (default) @ user-microservice ---
[INFO] ------------------------------------------------------------------------
[INFO] BUILD SUCCESS
[INFO] ------------------------------------------------------------------------
[INFO] Total time: 8.435 s
[INFO] Finished at: 2017-06-10T12:59:42+05:30
[INFO] Final Memory: 36M/324M
[INFO] ------------------------------------------------------------------------

```






/*****************************************************************************
************************************************************************
************************************************************************
** Running the JAR - java -jar target/user-microservice-0.0.1-SNAPSHOT.jar ***
************************************************************************
************************************************************************
******************************************************************************/
```
{Sat 10 Jun 13:02} ✘ -  ~/code_p/gatling/micro-services/ecommerce-microservices/user-microservice   master  java -jar target/user-microservice-0.0.1-SNAPSHOT.jar
2017-06-10 13:03:06.208  INFO 15803 --- [           main] c.d.p.UserMicroserviceApplication        : Starting UserMicroserviceApplication v0.0.1-SNAPSHOT on C02T41V3G8WL with PID 15803 (~/code_p/gatling/micro-services/ecommerce-microservices/user-microservice/target/user-microservice-0.0.1-SNAPSHOT.jar started by user in ~/code_p/gatling/micro-services/ecommerce-microservices/user-microservice)
2017-06-10 13:03:06.250  INFO 15803 --- [           main] s.c.a.AnnotationConfigApplicationContext : Refreshing org.springframework.context.annotation.AnnotationConfigApplicationContext@5415e2a7: startup date [Sat Jun 10 13:03:06 IST 2017]; root of context hierarchy
2017-06-10 13:03:06.416  INFO 15803 --- [           main] f.a.AutowiredAnnotationBeanPostProcessor : JSR-330 'javax.inject.Inject' annotation found and supported for autowiring
2017-06-10 13:03:06.658  INFO 15803 --- [           main] trationDelegate$BeanPostProcessorChecker : Bean 'encrypt.CONFIGURATION_PROPERTIES' of type [class org.springframework.cloud.bootstrap.encrypt.KeyProperties] is not eligible for getting processed by all BeanPostProcessors (for example: not eligible for auto-proxying)
2017-06-10 13:03:06.659  INFO 15803 --- [           main] trationDelegate$BeanPostProcessorChecker : Bean 'encryptionBootstrapConfiguration' of type [class org.springframework.cloud.bootstrap.encrypt.EncryptionBootstrapConfiguration$$EnhancerBySpringCGLIB$$430de1e1] is not eligible for getting processed by all BeanPostProcessors (for example: not eligible for auto-proxying)
2017-06-10 13:03:06.728  INFO 15803 --- [           main] c.d.p.UserMicroserviceApplication        : Started UserMicroserviceApplication in 0.775 seconds (JVM running for 1.373)

  .   ____          _            __ _ _
 /\\ / ___'_ __ _ _(_)_ __  __ _ \ \ \ \
( ( )\___ | '_ | '_| | '_ \/ _` | \ \ \ \
 \\/  ___)| |_)| | | | | || (_| |  ) ) ) )
  '  |____| .__|_| |_|_| |_\__, | / / / /
 =========|_|==============|___/=/_/_/_/
 :: Spring Boot ::        (v1.2.7.RELEASE)

2017-06-10 13:03:06.777  INFO 15803 --- [           main] ationConfigEmbeddedWebApplicationContext : Refreshing org.springframework.boot.context.embedded.AnnotationConfigEmbeddedWebApplicationContext@3f7dda5e: startup date [Sat Jun 10 13:03:06 IST 2017]; parent: org.springframework.context.annotation.AnnotationConfigApplicationContext@5415e2a7
2017-06-10 13:03:07.715  INFO 15803 --- [           main] o.s.b.f.s.DefaultListableBeanFactory     : Overriding bean definition for bean 'beanNameViewResolver': replacing [Root bean: class [null]; scope=; abstract=false; lazyInit=false; autowireMode=3; dependencyCheck=0; autowireCandidate=true; primary=false; factoryBeanName=org.springframework.boot.autoconfigure.web.ErrorMvcAutoConfiguration$WhitelabelErrorViewConfiguration; factoryMethodName=beanNameViewResolver; initMethodName=null; destroyMethodName=(inferred); defined in class path resource [org/springframework/boot/autoconfigure/web/ErrorMvcAutoConfiguration$WhitelabelErrorViewConfiguration.class]] with [Root bean: class [null]; scope=; abstract=false; lazyInit=false; autowireMode=3; dependencyCheck=0; autowireCandidate=true; primary=false; factoryBeanName=org.springframework.boot.autoconfigure.web.WebMvcAutoConfiguration$WebMvcAutoConfigurationAdapter; factoryMethodName=beanNameViewResolver; initMethodName=null; destroyMethodName=(inferred); defined in class path resource [org/springframework/boot/autoconfigure/web/WebMvcAutoConfiguration$WebMvcAutoConfigurationAdapter.class]]
2017-06-10 13:03:08.088  INFO 15803 --- [           main] o.s.b.f.s.DefaultListableBeanFactory     : Overriding bean definition for bean 'infoEndpoint': replacing [Root bean: class [null]; scope=; abstract=false; lazyInit=false; autowireMode=3; dependencyCheck=0; autowireCandidate=true; primary=false; factoryBeanName=org.springframework.boot.actuate.autoconfigure.EndpointAutoConfiguration; factoryMethodName=infoEndpoint; initMethodName=null; destroyMethodName=(inferred); defined in class path resource [org/springframework/boot/actuate/autoconfigure/EndpointAutoConfiguration.class]] with [Root bean: class [null]; scope=; abstract=false; lazyInit=false; autowireMode=3; dependencyCheck=0; autowireCandidate=true; primary=false; factoryBeanName=org.springframework.cloud.autoconfigure.RefreshAutoConfiguration$InfoEndpointRebinderConfiguration; factoryMethodName=infoEndpoint; initMethodName=null; destroyMethodName=(inferred); defined in class path resource [org/springframework/cloud/autoconfigure/RefreshAutoConfiguration$InfoEndpointRebinderConfiguration.class]]
2017-06-10 13:03:08.453  INFO 15803 --- [           main] o.s.cloud.context.scope.GenericScope     : BeanFactory id=c76cd8dd-6d6e-385d-be7c-6409189721f0
```



/**********************************************************************
************************************************************************
************************************************************************
** Running the Gatling test using Maven ***
************************************************************************
************************************************************************
************************************************************************/
```
{Sat 10 Jun 14:44} -  ~/code_p/gatling/micro-services/tests/user-microservice-gatling-tests   master ●  mvn clean gatling:execute
```


```
Installing Influxdb
{Sat 10 Jun 13:24} -  ~/code_p/gatling/micro-services   master ●  brew install influxdb
Updating Homebrew...
==> Auto-updated Homebrew!
Updated 1 tap (homebrew/core).
No changes to formulae.

==> Downloading https://homebrew.bintray.com/bottles/influxdb-1.2.4.sierra.bottle.tar.gz
######################################################################## 100.0%
==> Pouring influxdb-1.2.4.sierra.bottle.tar.gz
==> Using the sandbox
==> Caveats
To have launchd start influxdb now and restart at login:
  brew services start influxdb
Or, if you don't want/need a background service you can just run:
  influxd -config /usr/local/etc/influxdb.conf
==> Summary
🍺  /usr/local/Cellar/influxdb/1.2.4: 8 files, 44.2MB
{Sat 10 Jun 17:18} -  ~/code_p/gatling/micro-services   master ● 
```


********* GATLING --> INFLUXDB --> GRAFANA  *************


  influxd -config /usr/local/etc/influxdb.conf

  checkout - http://gatling.io/docs/current/realtime_monitoring/

  Graphite-InfluxDB-Grafana
Gatling can provide live metrics via the Graphite protocol which can be persisted and visualised.

The sections below describe how to configure Gatling with InfluxDB and Graphite, and use Grafana as a graphing library. We also present a lo-fi solution which prints parsed Graphite data to standard out.

********* GATLING.conf  *************
In the gatling.conf add “graphite” to the data writers and specify the host of the Carbon or InfluxDB server.
~/code_p/gatling/micro-services/tests/user-microservice-gatling-tests/src/test/resources/gatling.conf
```
data {
  writers = [console, file, graphite]
}

graphite {
  host = "192.0.2.235"  # InfluxDB or Carbon server
  # writeInterval = 1   # Default write interval of one second
}
```
new format
```
 data {
  writers = "console, file, graphite"
  graphite {
  host = "192.0.2.235"  # InfluxDB or Carbon server or 127.0.0.1
  # writeInterval = 1   # Default write interval of one second
  }
}
```


********* INFLUXDB  *************
InfluxDB
InfluxDB is one of the new crop of time-series databases [1]. It is self-contained, easy-to-install and resource efficient.

Install

Install InfluxDB through your package manager.

Graphite plugin

Add the below to the Graphite section of /etc/influxdb/influxdb.conf or /usr/local/etc/influxdb.conf
```
[[graphite]]
        enabled = true
        database = "gatlingdb"

        templates = [
                "gatling.*.*.*.* measurement.simulation.request.status.field",
                "gatling.*.users.*.* measurement.simulation.measurement.request.field"
     ]
```

********* START INFLUXDB using the config file  *************
```
influxd -config /usr/local/etc/influxdb.conf
```

********* START GRAFANA  *************
```
grafana-server --config=/usr/local/etc/grafana/grafana.ini --homepath /usr/local/share/grafana cfg:default.paths.logs=/usr/local/var/log/grafana cfg:default.paths.data=/usr/local/var/lib/grafana cfg:default.paths.plugins=/usr/local/var/lib/grafana/plugins
```

Grafana URL - http://;ocalhost:3000
admin/admin
