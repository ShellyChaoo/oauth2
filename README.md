---
description: Survey MoonBear provides a new way of survey services.
---

# Quick Start

### Resources

* [Github](https://github.com/SurveyMoonBear/SurveyMoonbear_APP)
* [Heroku](https://moonbear.herokuapp.com)
* [HackMD](https://hackmd.io/@WVFBeK-KRt-CDsNCu4hqdQ/r1u3-zSSt)

### Getting Started

#### Requirements

**Permissions**

* Collaborator of SurveyMoonBear organization in Github
* Collaborator of Heroku moonbear app

**Credentials**

* config/secrets.yml
* Moonbear Google Drive account & password

#### SETUP

**Run on local**

1. Clone the repo

```
$ git clone git@github.com:SurveyMoonBear/SurveyMoonbear_APP.git
```

1. Install gems

```
$ bundle install --without production
```

1. Add config/secret.yml file
2. Run DB migrations

```
$ rake db:migrate
$ RACK_ENV=test db:migrate
```

1. Run tests

```
$ rake spec
```

1. Run the app

```
$ rake run:dev
```

**Get Remote Access**

Create a Heroku remote to existing Heroku repo

```
$ heroku git:remote -a moonbear
```
