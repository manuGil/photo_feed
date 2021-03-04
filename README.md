# BUILD A PHOTO FEED USING DJANGO

This a Django app to  building a photo feed, and it was originally developed by [Samuel Ogundipe](https://github.com/samuelayo). The app is similar to instagram, but a stripped off version without the comments and like feature. The original tutorial can be found here : [https://pusher.com/tutorials/photo-feed-django/ ](https://pusher.com/tutorials/photo-feed-django/) 

## Getting Started

These instructions (for Windows) will get you a copy of the project up and running on your local machine for development and testing purposes. 

- Clone this repository by running: 
```shell
> git clone https://github.com/manuGil/photo_feed.git
```
- Change directory to the cloned repo
```shell
> cd photo_feed
```
- Create a Python virtual environment
```shell
> python -m venv C:\devel\photo_feed\venv
```
- Activate viertual environment and install required libraries: i.e pusher and django
```shell
# Activate virtualevironment
> venv\Scripts\activate 
(venv) > pip install django pusher
```
> If installing packages with pip finishes with errors. Run the last command a second or third time.

### Prerequisites

#### Setup Pusher (Not used in the Codig Session)

~~Replace the XXX_APP_ID, XXX_APP_KEY, XXX_APP_SECRET and XXX_APP_CLUSTER with your own keys you obtained when you created an app on Pusher in the line below in your `photofeed\views.py` file. If you dont have a Pusher account, sign up [here](Https://pusher.com)~~

```
Pusher(app_id=u'XXX_APP_ID', key=u'XXX_APP_KEY', secret=u'XXX_APP_SECRET', cluster=u'XXX_APP_CLUSTER')
```
~~Replace the XXX_APP_KEY and XXX_APP_CLUSTER with your app key and cluster respectively in the `feed\templates\index.html` file.~~

### Database Migrations
 - Run the following command at the root of your application to  make the migrations needed for the database. The root directory is where the file `manage.py` is
 
 ```shell
 python manage.py makemigrations
 ```
 
 - Run this command to migrate the database
 
 ```shell
  python manage.py migrate
 ```

And finally, start the application:

```
python manage.py runserver.
```
and visit http://localhost:8000/ to see the application in action.

## Built With

* [Pusher](https://pusher.com/) - APIs to enable devs building realtime features
* [DJango](https://docs.djangoproject.com/) - The web framework for perfectionists with deadlines. 
* [Jquery](https://jquery.com/) - The Write Less, Do More, JavaScript Library

