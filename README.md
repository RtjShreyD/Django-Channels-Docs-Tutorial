## Django Channels Tutotial repository from Official Docs

[Official Docs](https://channels.readthedocs.io/en/stable/index.html)
[Official Tutorial](https://channels.readthedocs.io/en/stable/tutorial/index.html)

#### Please note this repository is just for my references for future usage, refer to the official docs and official tutorial for proper explanation.

## To run the repo :

1. Create a virtualenv

`python3 -m venv env`

2. Activate the env

`source env/bin/activate`

3. Clone the Repository

`git clone https://github.com/RtjShreyD/Django-Channels-Docs-Tutorial.git`

4. Run 

`pip install -U pip`
`pip install -r requirements.txt`

5. Make sure to have Docker installed on system. Start a redis server so that we are able to use the channel layers where redis acts as its backing store.

`docker run -p 6379:6379 -d redis:5`

6. Run the asgi Django-channels server 

`python manage.py runserver`

7. Open two tabs in browser at http://127.0.0.1:8000/chat/ 

8. Enter the same room name in both the tabs and hit enter

9. Type any message in the long rectangular box above send and see the messsage appears on both tabs in the logs text box.

10. Thus demonstrated Django channels use websockets asynchronously in channel layers to send and receive messages. Synchronous implementation is also demonstrated in the Official tutorial.