# python-qa
A control quality to deliver clean code for small python projects with [pre-commit](https://pre-commit.com/#intro).

1. Install quality control tools in [requeriments-dev.txt](https://github.com/beotavalo/python-qa/blob/main/requirements-dev.txt)
   ```python
   pip install -r requirements-dev.txt
   ```
2. Add a pre-commit configuration, create a file named [.pre-commit-config.yaml](https://github.com/beotavalo/python-qa/blob/main/.pre-commit-config.yaml)
3. Install the git hook scripts to set up the git hook scripts

   ```bash
   pre-commit install
   ```
4.  (optional) Run against all the files

    It's usually a good idea to run the hooks against all of the files when adding new hooks (usually pre-commit will only run on the changed files during git hooks) and check if the new hooks is working

    ```bash
    pre-commit run --all-files
    ```
5. Once pre-commit is configured will run automaticaly all quality control test test [hooks] and  will not permit to run ```git commit -m 'mesage'``` if you not correct all errors and warnings. When you correct a script file. You should save changes and run again ```git add .``` and ```git commit -m 'mesage'```.

## References:
- [Simplify your Python Code: Automating Code Complexity Analysis with Wily](https://towardsdatascience.com/simplify-your-python-code-automating-code-complexity-analysis-with-wily-5c1e90c9a485/)
