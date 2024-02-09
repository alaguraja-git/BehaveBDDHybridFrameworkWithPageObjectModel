#BehaveBDDHybridFrameworkWithPageObjectModel

pip install -r requirements.txt

npm install -g allure-commandline

allure --version

python -m venv project path

eg:


python -m venv C:\PYTHON-BDD-FRAMEWORK\BehaveBDDHybridFrameworkWithPageObjectModel\venv

Ctrl+Shift+P ---> Select Interpretor

Select --> browse --> our vene--> inside enter interpradation path --> find --> venv --> script --> python.exe

----------------------------------------

WIndows:

python -m venv .venv


behave -f allure_behave.formatter:AllureFormatter -o Reports/ features

behave -f allure_behave.formatter:AllureFormatter -o %allure_result_folder% ./features

behave -n "scenario name"
eg:
behave -n "Login with valid credentials"

tags:

behave --tags=sanity

behave --tags=-sanity (means, except sanity it will run)

-------------------------------------------------------------

The minimum requirement for a features directory is:

features/
features/everything.feature
features/steps/
features/steps/steps.py
A more complex directory might look like:

features/
features/signup.feature
features/login.feature
features/account_details.feature
features/environment.py
features/steps/
features/steps/website.py
features/steps/utils.py

---------------------------------------------------

Tag selection on the command-line may be combined:

--tags="@wip or @slow"
This will select all the cases tagged either “wip” or “slow”.

--tags="@wip and @slow"
This will select all the cases tagged both “wip” and “slow”.

