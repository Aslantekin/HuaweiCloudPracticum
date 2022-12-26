#! /bin/bash
yum update -y
yum install python3 -y
pip3 install flask
pip3 install flask_mysql
TOKEN="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"
FOLDER="https://$TOKEN@raw.githubusercontent.com/Aslantekin/HuaweiCloudPracticum"
curl -s --create-dirs -o "/root/templates/index.html" -L "$FOLDER"/templates/index.html
curl -s --create-dirs -o "/root/templates/add-update.html" -L "$FOLDER"/templates/add-update.html
curl -s --create-dirs -o "/root/templates/delete.html" -L "$FOLDER"/templates/delete.html
curl -s --create-dirs -o "/root/phonebook-app.py" -L "$FOLDER"/phonebook-app.py
python3 /root/phonebook-app.py