zipkinΪ�ֲ�ʽ��·���ü��ϵͳ���ۺϸ�ҵ��ϵͳ�����ӳ����ݣ��ﵽ��·���ü�ظ��١�

mvn clean
mvn eclipse:clean
mvn eclipse:eclipse
mvn package

--����zipkin
java -jar zipkin-server-1.13.1-exec.jar
WebUI: http://127.0.0.1:9411/

--�������Է���
java -jar target/zipkin-brave-demo1-*.jar
java -jar target/zipkin-brave-demo1-*.jar --spring.profiles.active=service2
java -jar target/zipkin-brave-demo1-*.jar --spring.profiles.active=service3
java -jar target/zipkin-brave-demo1-*.jar --spring.profiles.active=service4

--����
��������URL��鿴zipkin��WebUI
http://localhost:8080/start
http://localhost:8080/foo
http://localhost:8080/bar
http://localhost:8080/tar

