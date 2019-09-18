I was able to hit multiple pods at once in Kubernets with this code and it is the solution for my question in SO: https://stackoverflow.com/questions/49612412/kubenetes-is-it-possible-to-hit-multiple-pods-with-a-single-request-in-kubernet

Apart from working as an agent to invalidate cache in multiple pods, Hazelcast in kubernetes can be used as an event listener.
This is a small POC for the same.

# HazelcastAsEventListener
Using Hazelcast ISet and event listeners for invalidating cache.
This project is to test event listener sequencing in a hazelcast cluster.

Update HazelcastConfig file. Add your local ip address.
I find intelliJ very convienient to start multiple servers on different ports. Start application multiple times by changing the port.

Hit the endpoint "http://localhost:9040/set?dataKeys=123456", and you can see the value getting propogated across multiple nodes.
