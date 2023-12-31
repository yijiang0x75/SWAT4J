# SWAT4J
System call allowlist for java container

## Dataset:
| Image | Version | Description | Download/Stars | Github Stars | Image Size |
| :-----| :-----| :-----| :-----| :-----| :-----|
| Tomcat | 7.0 | Web Application Servers | 500M+/3.5k | 6.7k | 382M |
| Jetty | 9.4.51 | Servlets and HTTP Servers | 10M+/399 | 3.6k | 378M |
| Orientdb | 3.2.19 | Multi-model NoSQL Database | 10M+/173 | 4.6k | 358M |
| Cassandra | 3.0.29 | Distributed NoSQL Database System | 100M+/1.5k | 8k | 296M |
| Elasticsearch | 7.5.2 | Search and Analytics Engine | 500M+/6.1k | 64k | 779M |
| Solr | 8.7.0 | Enterprise Search Application Server | 100M+/953 | 745 | 543M |
| Zookeeper | 3.4.14 | Distributed Coordination Service for Applications | 100M+/1.4k | 11.3k | 260M |
| Storm | 2.4.0 | Distributed Real-Time Computation System | 5M+/189 | 6.5k | 668M |
| Groovy | 4.0.0 | Dynamic Object-Oriented Scripting Language | 50M+/139 | 4.9k | 362M |
| Jruby | 9.4.2.0 | Ruby Interpreter Based on Java Platform | 10M+/113 | 3.7k | 299M |


## Code Analysis:
**/src/main/java/com/sspku/jtracer/bytecode_new/NewByteCodeTracer.java**

Code Analysis is currently for tomcat.
If you want to analyse other projects, you need to replace tomcat with the appropriate project in the java code and pom files.


## Cross Language Interface Dependency Analysis & Binary Analysis:
**binary_analyser.py**

Cross Language Interface Dependency Analysis & Binary Analysis is currently for tomcat. 
If you want to analyse other projects, you need to modify "native_methods" and function "build_xxx_map" in binary_analyser.py.

## Results:
  ### Native methods called by the container generated by code analysis:
  /result/static/code_analysis

  ### System calls obtained from different granularity analyses:
  /result/static/result_different_granularity/

  ### Results of static analysis:
  /result/static/result_final/

  ### Results of dynamic analysis:
  /result/dynamic/

  ### Combining and redundantly eliminating the results of static and dynamic analysis:
  /result/combine/
  
  ### CVEs Mitigated by SWAT4J:
  /result/combine/CVE/

  
         
