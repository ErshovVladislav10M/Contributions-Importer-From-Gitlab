# Contributions Importer from GitLab

This tool is based on Miro Mannino's [Contributions Importer for GitHub](https://github.com/miromannino/contributions-importer-for-github) to help users import contributions continuously via GitLab API.

<h3 align="center">

  ![2022_alpha_light_gitlab](https://user-images.githubusercontent.com/23136222/207664781-a0cb309d-9154-4b0d-8c6f-47d8f779ce6d.png#gh-light-mode-only)
  ![2022_alpha_dark_gitlab](https://user-images.githubusercontent.com/23136222/207656073-9767a871-55be-4446-ac4c-3c6e8387bd21.png#gh-dark-mode-only)
  ▼

  ![2022_alpha_light_github](https://user-images.githubusercontent.com/23136222/207667695-8ae40bef-4af9-469e-908f-26892b15ae7c.png#gh-light-mode-only)
  ![2022_alpha_dark_github](https://user-images.githubusercontent.com/23136222/207667690-b853ccd7-8ab6-4000-8f69-cfc0f0faa585.png#gh-dark-mode-only)
</h3>

# How it Works

Login to GitHub with your personal access token to get your username, primary email and clone the mock repository. Read the last mock commit date to count from. After that, authorize with a personal access token for each GitLab server to get a list of projects with developer permissions changed since our date via the API. Requests all user commits since our date for each project and sort them by date for backwards compatibility. Then parse each commit to get a list of changed file types with insertion and deletion counts. At the end, this data is sent to the original importer to create new mock commits. All changes are pushed to GitHub before exit.

# How to Use

<p align="center">
  
  ![alpha_light_token](https://user-images.githubusercontent.com/23136222/208074919-f9c9bc7d-db0a-4cad-a3e2-0b34e8898682.png#gh-light-mode-only)
  ![alpha_dark_token](https://user-images.githubusercontent.com/23136222/208074913-443edec5-7546-4a24-9759-c5aed279f9c1.png#gh-dark-mode-only)
</p>

<p align="center">

  ![alpha_light_secrets](https://user-images.githubusercontent.com/23136222/207987066-d25e9051-3161-4d93-938c-5e9c1eab7aea.png#gh-light-mode-only)
  ![alpha_dark_secrets](https://user-images.githubusercontent.com/23136222/207987065-8f0aacc4-3fea-416f-8abc-124d6b7d8c8b.png#gh-dark-mode-only)
</p>
