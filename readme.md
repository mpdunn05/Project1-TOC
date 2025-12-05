Overview: These instructions provide you with a skeleton python definition for each problem type. After cloning this repo, you will modify only those functions that you have signed up for (at most 3 for a three person group)
* You will clone a repo that has skeleton code for each possible program.
* You will modify the body of your selected code for your implementation. Do not change the arguments.
* Your output can be simply printed to screen for visual inspection. but while we grade this assignment, we will use have our custom test case files and see if we are able to see results as expected.
* Instructions are also included on running your code when you want to test it.
* When you modified code is called the arguments to the function on each call provide a test case (you do not need to read test cases rom any files with this procedure).
* The "input" folder holds the test cases that the above mechanism will use when you run your tests.
* The test cases to be used for grading are separate, and are not visible to you.
* If you need to access other python packages in your code, the UV package discussed below can give your functions access to them.
* Send all questions about this infrastructure to Laxminarayana Vadnala lvadnala@nd.edu

<!-- ## instructions to generate a PAT (a Personal Access Token): -->


<!-- * Go to GitHub → Settings → Developer settings → Personal access tokens → Tokens (classic)
* Click "Generate new token" → "Generate new token (classic)"
* Set expiration (90 days recommended)
* Select scopes: repo (full control of private repositories)
* Generate token and copy it -->


## Student Instructions to clone the repository and how to run and finally submit the assignment:
------------------
* From your browser, go to [GITHUB URL](https://github.com/pkogge/Project1-TOC) and click the fork button as shown in the picture below


![fork_button](documentation/assets/fork_button.png "fork button")


* You will now enter the fork screen, from here make sure to select your own github account which is highlighted in screen below (for instance, I have selected my own personal account), after that click on the `create fork` button highlighted in orange arrow and box.

![fork_screen](documentation/assets/fork_screen.png "fork screen")

* You will now see the screen which looks like below, the first red box on left should reflect your own github account and should say forked from `forked from pkogge/Project1-TOC.` Then you can follow general instructions of cloning the github repository. Here is the [Docs Link](https://docs.github.com/en/repositories/creating-and-managing-repositories/cloning-a-repository) that can help you to clone the github repository on your computer.

![cloned_repo](documentation/assets/cloned_repo.png "cloned_repo")

* Once you clone the repository, open the project in the IDE of your choice.

### Getting started with the python support package manager "UV" installation.
----------------

* Start  by installing `UV` in your machine. Here is the [instructions page](https://docs.astral.sh/uv/getting-started/installation/#__tabbed_1_1) that helps you to install the `UV`.

* Immediately after installing it run command `uv sync` which installs the pytests and other required packages.

* NOTE: If you are struggling with installing `UV` please feel to reach me out via slack, I can help you navigate. lvadnala@nd.edu

* This project template is equipped with all the packages required for your project. No additional python packages are required to be installed, but if you want to install additional python packages make sure use the command `uv add <python-package-name>` (mostly it is not useful).

### How can we run the code using UV when other packages are needed
----------------
* For this project I am using UV to demonstrate to run the code. Basically you need to use the command `uv run main.py <filename> <input_string>` from the root of the project folder in the terminal to see your code executes. eg., `uv run main.py ./input/aplus.csv "aaaa"`
* Immediately after cloning the repository, and you didnt do any code changes, if you run the command `uv run main.py ./input/aplus.csv "aaaa"` you would see the results below.

```
(base) lax@Mac Project1-TOC % uv run main.py ./input/aplus.csv "aaaa"
Tracing NTM: a plus on input 'aaaa'
```

* the `Tracing NTM: a plus on input 'aaaa'` message states that you are good to make changes to the code.

### Making changes to the code and running the test cases of your own
----------------

* Here is the folder structure that every student should make changes to. This is personalized for SAT, but the others are similar. The src directory hold the code you want to modify.

```
.
|── src/
│   |── entrypoint.py
|   |── ktape_dtm.py
|   |-- ntm_tracer.py
|   |── input/
|   |   |-- aplus.csv
|   |   |-- ktape.csv
|   |   |-- ntm_n1n.csv
|-- main.py
```

* The `src/entrypoint.py` file contains the function called as `main.` Make sure to add all your auxikiary files into the `src` folder and make sure to use the `entrypoint.py` file's main function as your main function Dont change this structure as if you do the automation wont be able to perform the grading.
* The `input` folder is where you will find sample inputs for to get started for project.
* The `module_tests` is the folder where you can add your own custom test cases. If you are familiar with pytests you can do so, but it is not compulsory to add test cases to the project, its totally the students choice to add, since the pytests have a little learning curve.
* `main.py` please dont edit this file, this is the main file and it should stay like this.

### Commit the code and make sure to raise a PR (Pull Request)
---------------

* Push the changes to the repositiory. Here is the [Docs Link](https://docs.github.com/en/get-started/using-git/pushing-commits-to-a-remote-repository) that helps you with basic git commands to push the code.
* Now the last step is to raise the PR to the Forked repo, here is the [Docs link](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request-from-a-fork)
* Please update the PR link to the [Teams Spread Sheet](https://docs.google.com/spreadsheets/d/1FYyJMDnft__n0SohcIcSL7lUO60RMtJk9nuVJ5l30SY/edit?usp=sharing) shared by Dr. Kogge. This is most important since we grade only the links that are part of the teams spreadsheet.
