
#  Social Account Authentication Using Django-allauth

This is a simple web application where users can sign in with their social accounts like Google, Facebook, GitHub.

 ##  _Documentation_  
 
[https://django-allauth.readthedocs.io/en/latest/](https://django-allauth.readthedocs.io/en/latest/)


## Providers Used
The below OAuth2 providers are used in this application
* Google
* Facebook
* GitHub
## Run Locally

Clone the project

```bash
  git clone https://github.com/Shivakumar1V/Social-Account-Signin-Using-Django-allauth
```

Install dependencies

```bash
  pip install -r requirements.txt
```

Create a superuser with the below command
```bash 
  python manage.py createsuperuser
```

Start the server

```bash
  python manage.py runserver
```

- It will run the application on [localhost:8000](http://localhost:8000)

## Get Client id and Secret key 
Get your `Client id` and `Secret key` by registering app on the providers website by following the below docs
* Google: [https://django-allauth.readthedocs.io/en/latest/providers.html#google](https://django-allauth.readthedocs.io/en/latest/providers.html#google)
* Facebook: [https://django-allauth.readthedocs.io/en/latest/providers.html#facebook](https://django-allauth.readthedocs.io/en/latest/providers.html#facebook)
* GitHub: [https://django-allauth.readthedocs.io/en/latest/providers.html#github](https://django-allauth.readthedocs.io/en/latest/providers.html#github)  
__Note:__ Use `http://localhost:8000` as domain name while registering app as this project running on `http://localhost:8000` 


## Add Social Application
For adding Social Application follow the below steps
- Open the browser and visit [http://localhost:8000/admin/socialaccount/socialapp/add/](http://localhost:8000/admin/socialaccount/socialapp/add/) 
- Login with `admin` Username and Password
- Select **Provider**, type provider name in the **Name** section, enter your **Client id** and **Secret key**, add **localhost:8000** to **Chosen sites** and click on **save** - continue this with all providers(Google, Facebook, GitHub)

**Yeah!** Now the application is ready to use  
Go to **[http://localhost:8000](http://localhost:8000)** and enjoy the application