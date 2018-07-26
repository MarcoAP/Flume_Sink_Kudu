# Flume_Sink_Kudu
Como criar um Agent Flume realizando um Source em SpoolDir e um Sink em uma tabela no database Apache Kudu

# Jar no Git do Kudu Sink para se colocar na pasta Lib do FLUME
$ git clone -b branch-1.1.x https://github.com/apache/kudu.git

# Geração de pacote Jar novo após fazer download do SINK FLUME do Git
$ mvn package -DskipTests

# Chamada no agent
$ flume-ng agent -n agent -f /home/TC014550/flume/test2/agent.prop -c /etc/flume-ng/conf/*

