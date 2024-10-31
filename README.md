# IITM_TDS_PROJECT1
# GitHub User and Repository Scraping in Zurich

- I used the GitHub API to collect detailed data on Zurich-based users with over 50 followers and their most recent public repositories, processing and storing it in structured CSV files.
- The most surprising insight was that **a significant portion of Zurich developers actively contribute to open-source projects in diverse languages, yet a high percentage lack licenses in their repositories**.
- Based on this data, **I recommend developers add clear licensing to their repositories to enhance project credibility and usability for collaborators**.

## Project Overview

This project involves scraping data on active GitHub users in Zurich who have a minimum of 50 followers, along with information about their recent public repositories. The objective is to store user and repository data in two structured CSV files, `users.csv` and `repositories.csv`, while cleaning and standardizing fields for consistent data analysis.

### Data Collection Process

1. **User Data:** For each eligible user (over 50 followers), we captured details such as `login`, `name`, `company`, `location`, `email`, `hireable`, `bio`, `public_repos`, `followers`, `following`, and `created_at`.
   - **Company Data Cleaning**: All company names were stripped of leading whitespace, the `@` symbol (only the first occurrence), and converted to uppercase for consistency.
   
2. **Repository Data:** For each user, up to 500 of their most recently pushed public repositories were collected with fields: `login`, `full_name`, `created_at`, `stargazers_count`, `watchers_count`, `language`, `has_projects`, `has_wiki`, and `license_name`.
   
3. **Data Storage:** The data was stored in `users.csv` for user information and `repositories.csv` for repository details. Each file was designed to allow easy querying and analysis.

### Analysis and Findings

A high-level examination of the data uncovered trends and patterns among developers in Zurich:
- **Open Source Participation:** Many developers engage in open-source contributions, often using a variety of programming languages, suggesting a vibrant and diverse developer community in Zurich.
- **Licensing Practices:** An observation was made that a large percentage of repositories lack specified licenses, which could limit usage and discourage contributions from other developers.

### Recommendations

1. **License Your Code**: Adding a license to your repositories helps protect your work and encourages collaboration.
2. **Profile Visibility**: Developers may benefit from updating their profile with bio and company information, as it can enhance their professional presence.
3. **Project Setup**: Enabling projects and wikis in repositories can make it easier for collaborators to get involved and understand the project’s goals.

### Files in Repository

- **users.csv**: Contains user information with fields as specified in the project.
- **repositories.csv**: Contains up to 500 of the most recent repositories for each user.

Thank you for reviewing this project! Your feedback is appreciated and will help improve future data collection and analysis practices.
