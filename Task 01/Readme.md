Prepare simple HTTP server

- That serves folder “content” in a working dir as a root
- index.html should be served as /
- Can be NGINX with a few lines of additional configuration
Create a Dockerfile for it
- It should expose port 8080
- “content” dir should be attached as a volume
- Depending on a build-arg IS_READY generate two different index.html
- If IS_READY true – with text “We are ready”
- If IS_READY false – with text “We are not ready”
- That index.html should replace default in “content” after start
