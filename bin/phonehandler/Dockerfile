FROM python:3.8.2
LABEL maintainer="Sashwat K <sashwat0001@gmail.com>"

# Update and upgrade linux container
RUN apt-get -y update
RUN apt-get upgrade -y

# Clone Trivandrum phonebook API handler
RUN git clone https://github.com/sashuu6/trivandrum-phonebook-api_handler.git /usr/share/phonehandler/

# Requirements.txt
RUN pip3 install -r /usr/share/phonehandler/requirements.txt

# Autoremove unnecessary tools
RUN apt-get autoremove -y

# Runs app.py
ENV FLASK_APP /usr/share/phonehandler/app.py
ENV FLASK_RUN_HOST 0.0.0.0
CMD ["flask", "run"]