FROM ubuntu:latest

WORKDIR /app

COPY . .

# ca-certificates is needed to make HTTPS requests from a Unity client.
RUN ["apt", "update"]
RUN ["apt", "install", "ca-certificates", "-y"]

EXPOSE 10771

# RUN ["chmod", "+x", "./LinuxServer.x86_64"]
CMD ["./LinuxServer.x86_64", "-nographics", "-batchmode", "--port=10771"]

