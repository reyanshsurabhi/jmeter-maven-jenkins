Create the maven project
mvn archetype:generate -DgroupId=com.example -DartifactId=jmeter-testproject -DarchetypeArtifactId=maven-archetype-quickstart -DinteractiveMode=false

to run as a jmeter file
.\jmeter-testproject\src\test\jmeter\simpletest1> jmeter -n -Jnumber_of_users=1 -Jloop_count_duration=30 -Japi_uri=google.com -t simpletest.jmx -l simple.jtl  -o .\reports\

generate a report from a .jtl
jmeter -g simple.jtl -o .\reports\

to run as a maven project

