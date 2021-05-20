mafia chatting environment


setup:
1. clone the repo
1.5. make a virtual environment(optional)
2. pip3 install -r requirements.txt
3. install docker
4. use the command in beckend/notes.txt to run redis
5. then run the command to start a server

6. in case you want to deploy, either port forward, or use a VM, with daphne/django-default-server for hosting

usage:
0. change the roles_dict in backend/backendsite/chat/consumers.py as per requirement
1. go to the server-homepage, add /chat to the url
2. enter your alias for the game
3. you will recieve your role
4. normal players can chat in the room
5. roles like mafia and detective's chat is common between all people of the same role
6. civilian chat is only visible to the civilian, so for other roles that aren't supposed to communicate
7. normal people can @god to communicate to god. eg.
    kill berlin@god (sent by mafia)
8. god can communicate to all people of a specific role. eg.
    whom to kill@mafia, or, whom to save@clueless_doctor
9. if somone dies, type dead@god to leave current room, and join dead chat