# Magento v2.3 Open Source Docker

## Requirements

- Docker Installation
- Docker Compose Installation
- GIT client installation

## Instructions

Clone this repo to your local.

```git clone https://github.com/trydock/docker-magento23.git```

Then navigate into the newly cloned directory `docker-magento23`

```cd docker-magento23```

Create a directory named `htdocs` inside the `docker-magento23` directory.

```mkdir htdocs```

Now copy the Magento 2.3 source code into the `htdocs` directory, then issue.

```chmod -R 777 htdocs```

Check and confirm the `.env` file and adjust the username and passwords if you feel so.

```cat .env```

The config files are located in the config files, Please review the same.

``` ls -lR configs```

Once in the directory `docker-magento23` and satisfied with the config files, please issue :

```docker-compose up -d```

Once the above command completes successfuly, launch a browser window and try the URL:

```http://localhost/```

Please note : If you are running, WAMP, XAMPP, MAMP, LAMP, LEMP etc on your local instance, then the port 80, 3306 might be alreday in use and may conflict with this docker setup. It is advised to stop your local web/db instances before starting this docker setup.

Once you are able to see the Magento Install Wizard, please complete the installation.

When asked for creating a admin user, store the credentials in a safe location for further reference.

Thanks,
debuggerboy
