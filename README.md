# thelouge-traefik

[The lounge](https://thelounge.chat/) with traefik in docker and docker-compose

![image](https://thelounge.chat/img/thelounge-screenshot.png)

## Installation

Clone the repo
```Shell
$ git clone https://github.com/pierre-emmanuelJ/thelounge-traefik.git
```
```Shell
$ cd thelounge-traefik
```
```Shell
$ touch acme.json && chmod 600 acme.json
```

In `docker-compose.yml` and `traefik.toml` replace `irc.example.xyz` by your desired domain.

```Shell
$ docker-compose up -d
```

Add a new user to use your The lounge client

```Shell
$ docker-compose exec thelounge /bin/bash
$ thelounge add <user-example>
2019-10-28 19:59:11 [PROMPT] Enter password: <password-example>
2019-10-28 19:54:01 [PROMPT] Save logs to disk? (yes) <yes | no>
2019-10-28 19:54:05 [INFO] User user-example created.
2019-10-28 19:54:05 [INFO] User file located at /var/opt/thelounge/users/user-example.json. 
```

Then you can access to your web IRC client on `irc.example.xyz`
![image](https://i.imgur.com/4J5s4a0.png)

:rocket: You can connect to an IRC server!
![image](https://i.imgur.com/W1GYJOa.png)

For the rest of the lounge functionalities see [thelounge doc](https://thelounge.chat/docs/)



## Enjoy
