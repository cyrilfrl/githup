#githup - PyPI Module
###Description
githup is a Python module that simplifies the process of interacting with GitHub repositories. It provides easy-to-use functions for downloading repositories, initializing repositories, and making commits.

##Installation
You can install the githup module from PyPI using pip. Open your terminal or command prompt and run the following command:
```python
pip install githup
```
##Download a Repository
To download a GitHub repository, you can use the download_repo function. By default, the repository will be saved in the current directory of the program file. Here's an example of how to use the function:
```python
import githup as gp

gp.download_repo("https://github.com/cyrilfrl/githup")
```
If you want to save the repository in a specific folder, you can provide the folder_path parameter, like this:
```python
import githup as gp

gp.download_repo("https://github.com/cyrilfrl/githup", "folder_path")
```
Replace folder_path with the actual path where you want to save the repository.

##Initiate a Repository
To initialize a new GitHub repository, you can use the init_repo function. Here's an example of how to use it:
```python
import githup as gp

gp.init_repo(github_repository_url, folder_path="local")
```
If you want to include a README.md file during initialization, you can add the add_readme parameter, like this:
```python
import githup as gp

gp.init_repo(github_repository_url, add_readme="readme")
```
You can also choose a specific folder to initialize the repository by providing the folder_path parameter with your desired path.

##Make a Commit
To make a commit to the GitHub repository, you can use the commit_files function. Here's how you can use it:
```python
import githup as gp

gp.commit_files(branch_name, commit_message, folder_path="local")
```
- branch_name: The name of the branch on which you want to commit.
- commit_message: The message you want to include when pushing your changes to the repository.
- folder_path: The default value is set to "local," which will commit the changes in the current folder where your Python program is located to GitHub.

##Note
The function names and parameters used in the examples above are clear and self-explanatory. If you still have questions about their usage, refer to the descriptions provided.

Thank you for using githup! I hope you find it useful for your projects. If you have any feedback or suggestions, feel free to share them. Happy coding!
