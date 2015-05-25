Semantic Content Management

Extends traditional content management systems with semantic services. Other feasible use cases include: direct usage from web applications (e.g. for tag extraction/suggestion; or text completion in search fields), 'smart' content workflows or email routing based on extracted entities, topics, etc.

To start:

    java -Xmx1024m -XX:MaxPermSize=256M -jar \
        target/org.apache.stanbol.launchers.full-*-SNAPSHOT.jar

So that you can POST content using, for example:

% curl -X POST -H "Accept: text/turtle" -H "Content-type: application/ld+json" \
     --data "The semantic enhancer can detect famous cities such as Paris and people such as Bob Marley." \
     http://semantic.teode.com/enhancer
