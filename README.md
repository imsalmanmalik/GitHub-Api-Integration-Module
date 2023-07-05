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

If fewer than 2 arguments are passed, the script will raise an error and display a usage message.



Above is a screenshot of the terminal showing an example where the script is executed with fewer than 2 arguments, resulting in an error message.



Above is a screenshot of the terminal showing the execution of the shell script. The password environment variable is set, and the script is run with the appropriate arguments to retrieve information about a specific repository.

## Additional REST Expressions

Here are a few more examples of REST expressions you can use with the shell script:

1. /repos/{owner}/{repo}: Get information about a specific repository.<b>
2. /orgs/{org}/repos: List repositories for a specific organization.<b>
3. /user/repos: List repositories for the authenticated user.<b>
4. /search/repositories?q={query}: Search repositories based on specific criteria.<b>
5. /repos/{owner}/{repo}/branches: Get the list of branches for a specific repository.<b>
6. Refer to the GitHub API documentation for more details on available endpoints and their usage.<b>

