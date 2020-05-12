FROM python:3.8.2
LABEL maintainer="Sashwat K <sashwat0001@gmail.com>"

# Update and upgrade linux container
RUN apt-get -y update
RUN apt-get upgrade -y

# Clone Trivandrum phonebook API handler
RUN https://github.com/sashuu6/trivandrum-phonebook-api_handler.git /usr/share/webhandler/

# Autoremove unnecessary tools
RUN apt-get autoremove -y

# Runs app.py
# EXPOSE 5000
# ENTRYPOINT ["python3"]
# CMD ["/usr/share/webhandler/app.py"]