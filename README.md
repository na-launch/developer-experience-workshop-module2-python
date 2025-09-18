# 🚀 **Module 2: Introduction to DevSpaces**

**Technology Stack:**

- Python
- DevSpaces  

---

## 🎯 **Scenario**

Inside your workspace is a very simple Python Application built using Flask. The application returns a “hello world” based on the language you choose for it.

The country is based on a 2-letter country code.  
For example, `countrycode=IT` will output “ciao mondo” (IT is for Italy).  

You can find all the mappings in the `translate.json` file, located in your `resources` folder.  
There is also a timestamp after the “hello world” message.

---

## 🐾 **Guided Walkthrough**

The application has some problems that we would like you to fix:

1. Run `pip install -r requirements.txt` to install the necessary dependencies
2. Your tests will not run with pytest because your environment variables are not set, please set the 3 items below
  - 2.1. `FLASK_APP=app.py`
  - 2.2. `FLASK_ENV=development`
  - 2.3. `PYTHONPATH=.`
3. Format the hello timestamp to use Eastern Standard Time (New York time)
4. Format the hello timestamp to display as {HH:MM MM/DD/YYYY}
5. Write a test case that tests both the timezone and the new date format
6. In `/routes/main.py` create a new route that will route to `/api/query`
  - 6.1. The request should be a GET method
  - 6.2. Append a query string to take an argument for the country code (e.g `/api/query?countryCode=en`) and set the API to return the correct greeting based on the country used in the querystring
7. Final Compilation

  ```python
  In a new terminal, run the App in flask (not python), use these settings
  flask run --host=0.0.0.0 --port=8080
  
  Open a Second terminal - and run pytest to ensure all test cases are passing
  ./pytest
  ```

---

## 🧩 **Challenge**

- [ ] Add an /api/magic8 endpoint that returns a random country code (like a magic 8-ball) and returns a random hello world greeting
- [ ] Write additional tests for /api/query and /api/magic8
- [ ] Add an additional end point for /api/query which functions the same but uses POST instead, use curl to test.
- [ ] Attach a simple stylesheet that will change the background color to blue
- [ ] Put the hello world inside a HTML `<blockquote>` tag - add color in the stylesheet to emphasize the blockquote area - (use render_template)
- [ ] Your styles.css can be kept in a new folder named /static (you can create)
- [ ] Your html files can be kept in a new folder named /templates (you can create)

---

## 🥚 **Easter Eggs!**

- [ ] There is an easter egg in the code
  - Be thorough! Look through the code..
  - Find and Solve the Golden Egg (it’s a 2 step process)

---

## ✅ **Key Takeaways**

- First look at Dev Spaces
- Familiarized yourself with setting up a Python App in Dev Spaces
- Took advantage of ‘quick build’ python apps in a container
- Using environment variables in your application
- Used your first OpenShift Service / Route!
