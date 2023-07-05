# GitHub API Shell Script

This shell script allows users to communicate with the GitHub API and retrieve information from repositories. It provides a simple and efficient way to make API calls and obtain data from GitHub.

## Prerequisites

- cURL: Make sure you have cURL installed on your system. You can install it using package managers like Homebrew (`brew install curl`) or MacPorts (`sudo port install curl`).

## Usage

1. Export the GitHub Access Token as an environment variable in your terminal session:
   
```shell
export password=YOUR_GITHUB_ACCESS_TOKEN
```

Replace YOUR_GITHUB_ACCESS_TOKEN with your actual GitHub access token. This sets the password environment variable to your token.

Run the shell script, providing the necessary arguments:

```shell
./github_script.sh $password [REST expression]
Replace [REST expression] with the specific REST expression for the GitHub API you want to use.
```

If fewer than 2 arguments are passed, the script will raise an error and display a usage message as shown below:


<img width="1280" alt="Screenshot 2023-07-05 at 7 57 17 PM" src="https://github.com/imsalmanmalik/GitHub-Api-Integration-Module/assets/121328365/f4b815dc-14ea-47e2-94a9-0ae69673ec3b">



Below is a screenshot of the terminal showing the execution of the shell script. The password environment variable is set, and the script is run with the appropriate arguments to retrieve information about a specific repository.


<img width="1280" alt="Screenshot 2023-07-05 at 7 46 32 PM" src="https://github.com/imsalmanmalik/GitHub-Api-Integration-Module/assets/121328365/0eea9d27-96bd-4cb3-92ee-ea90e3f7ccf8">



## Additional REST Expressions

Here are a few more examples of REST expressions you can use with the shell script:

1. /repos/{owner}/{repo}: Get information about a specific repository.<b>
2. /orgs/{org}/repos: List repositories for a specific organization.<b>
3. /user/repos: List repositories for the authenticated user.<b>
4. /search/repositories?q={query}: Search repositories based on specific criteria.<b>
5. /repos/{owner}/{repo}/branches: Get the list of branches for a specific repository.<b>
6. Refer to the GitHub API documentation for more details on available endpoints and their usage.<b>

