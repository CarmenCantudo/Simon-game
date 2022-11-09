# Gitpod Reminders

To run a frontend (HTML, CSS, Javascript only) application in Gitpod, in the terminal, type:

`python3 -m http.server`

A blue button should appear to click: _Make Public_,

Another blue button should appear to click: _Open Browser_.

To run a backend Python file, type `python3 app.py`, if your Python file is named `app.py` of course.

A blue button should appear to click: _Make Public_,

Another blue button should appear to click: _Open Browser_.

In Gitpod you have superuser security privileges by default. Therefore you do not need to use the `sudo` (superuser do) command in the bash terminal in any of the lessons.


# Install Jest

`npm init`

No need to answer anything except:

test command: jest

`npm install --save-dev jest@26.6.3`


# Test in terminal

`npm test`


## Problems

If the terminal says: 

  `> jest-testing@1.0.0 test`

  `> echo "Error: no test specified" && exit 1`

> Error: no test specified


Add the following section to your package.json:

`{`

`  "scripts": {`

`    "test": "jest"`

`   }`

`}`

# Update

Due to a change in Jest's default configuration, you need to add the following code to the top of your test file:

`/**`

` * @jest-environment jsdom`

` */`

Your tests will break if you do not add this block. We have already added it to the starter files, but you will not see this code in the videos.
