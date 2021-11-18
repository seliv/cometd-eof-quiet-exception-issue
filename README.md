# cometd-eof-quiet-exception-issue
Minimal demo for CometD EofException-QuietException issue.

Run Java server with `mvn jetty:run` command. 
Use a browser (Google Chrome) to access web app at `http://localhost:8080/`.
Wait till server starts sending a flood of messages to the client and close the page.
Observe the issue (`org.eclipse.jetty.io.EofException` logged at `INFO` logging level).
