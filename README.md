# GitHub User Activity CLI

This is a simple command-line application that fetches and displays the recent public activity of a specified GitHub user using the GitHub API. The application runs from the command line, accepts a GitHub username as an argument, and handles errors gracefully.

Task from : https://roadmap.sh/projects/github-user-activity

## Features

- **Fetch Recent GitHub Activity**: Retrieves up to 10 of the most recent public events for a specified GitHub user.
- **Command-Line Usage**: Runs entirely from the command line, accepting a GitHub username as input.
- **Error Handling**: Provides meaningful error messages for invalid usernames, API failures, or connectivity issues.

## Requirements

- Python 3.x
- Internet connection

## How It Works

The script uses the GitHub API to fetch the public activity of a user:
- Sends an HTTPS `GET` request to GitHub's `https://api.github.com/users/{username}/events/public` endpoint.
- Processes the JSON response to retrieve event details, such as the type of event and the repository name.
- Displays up to 10 of the user’s most recent events in the terminal.

## Usage

1. **Clone or Download the Project**:
    ```bash
    git clone https://github.com/Rifatkazak/Projects-Task-Tracker.git
    cd Projects-Task-Tracker
    ```

2. **Run the Script**:
    Use the following command format to run the script:
    ```bash
    python Github_user_activity.py <github_username>
    ```

### Examples

```bash
# Fetch recent activity for the user 'cat'
python Github_user_activity.py cat
