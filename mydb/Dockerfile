FROM mongo

COPY users.json /users.json
COPY responses.json /responses.json
COPY questions.json /questions.json
CMD mongoimport --host mongo --db dockerdb --collection users --type json --file /users.json --jsonArray && mongoimport --host mongo --db dockerdb --collection responses --type json --file /responses.json --jsonArray && mongoimport --host mongo --db dockerdb --collection questions --type json --file /questions.json --jsonArray