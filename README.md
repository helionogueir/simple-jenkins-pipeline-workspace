# Simple Jenkins Pipeline Workspace
Simple Jenkins Pipeline Workspace

## Get Start
All instruction below was executed at Linux OS. Remember that you need to have [git](https://git-scm.com/downloads), [docker](https://docs.docker.com/install/#supported-platforms) and [docker-compose](https://docs.docker.com/compose/install/) installed.

### Up Environment
Execute the steps below:
```bash
mkdir -p "${HOME}/workspace"
cd "${HOME}/workspace"
# if it doesn't work! Go to git repository and use the HTTP version
git clone git@github.com:helionogueir/simple-jenkins-pipeline-workspace.git
docker-compose up
```

### Setup Jenkins
__\#1__ - After execute __docker-compose up__ you'll see the follow text:
```bash
*************************************************************
*************************************************************
*************************************************************

Jenkins initial setup is required. An admin user has been created and a password generated.
Please use the following password to proceed to installation:

f65baf02ab354ea5a994b5bb6b0365c8

This may also be found at: /var/jenkins_home/secrets/initialAdminPassword

*************************************************************
*************************************************************
*************************************************************
```
__\#2__ - Ok. Now you need copy _(ctrl + c)_ the code ***f65baf02ab354ea5a994b5bb6b0365c8*** in bash. Remember this code will be diferente in each instalation.

__\#3__ - Open your browser and access the address _[http://localhost:8080/](http://localhost:8080/)_. You'll see the follow page.

![Unlock Jenkins](.image/step-3.png)

__\#4__ - Paste _(ctrl + v)_ the code _(Ex: f65baf02ab354ea5a994b5bb6b0365c8)_ in field ***Administrator password***. Then click in ***Continue*** button.

__\#5__ - Nice! Click in ***Install suggested plugins*** button.

![Customize Jenkins](.image/step-5-1.png)

Waiting the installation to finish.

![Getting Started](.image/step-5-2.png)

__\#6__ - Fill the form informations and click in ***Save and Continue*** button.

![Create First User Admin](.image/step-6-1.png)

Click in ***Save and Finsish*** button.

![Instance Configuration](.image/step-6-2.png)

Click in ***Start using Jenkins*** button.

![Jenkins is ready](.image/step-6-3.png)

Great! Jenkins is installed and ready.

![Welcome to Jenkins](.image/step-6-4.png)

Now access [http://localhost:8088/](http://localhost:8088/) in your browser.