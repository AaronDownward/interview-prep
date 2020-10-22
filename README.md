# interview-prep

# build jenkins server container
docker build -t aarondownward/interview-jenkins jenkins
docker run -v //var/run/docker.sock:/var/run/docker.sock -p 8081:8080 --name jenkins aarondownward/interview-jenkins
docker exec -it jenkins bash
cd /var/run
chmod 777 docker.sock (not necessary as root user)

# create webhook
to do locally you can use ngrok to tunnel to localhost
documentation is fairly straightforward on website

testing webhook again

