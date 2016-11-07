
Original project (http://www.lightbend.com/activator/template/akka-dddd-cqrs)

docker run --name my-cassandra -d -p 9042:9042 cassandra:latest



sbt 'runMain com.boldradius.cqrs.ClusterNodeApp 127.0.0.1 2551'

sbt 'runMain com.boldradius.cqrs.ClusterNodeApp 127.0.0.1 2552'

sbt 'runMain com.boldradius.cqrs.HttpApp 127.0.0.1 9000 127.0.0.1 0'
