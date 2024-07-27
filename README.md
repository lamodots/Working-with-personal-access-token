# Generate a New Personal Access Token

  -  Step 1  Log in to GitHub with the your account.
  -  Step 2  Navigate to the Personal Access Tokens page:
       -  Go to your GitHub account settings.
        -  Click on "Developer settings" in the sidebar.
        -  Click on "Personal access tokens".
        -  Click on "Tokens (classic)" or "Fine-grained tokens" depending on what you are using.
        -  Click on "Generate new token" (or "Generate new token (classic)").
    -  Step 3  Configure the Token:
        -  Give your token a descriptive name.
        -  Select the scopes or permissions you need. Typically, repo for full control of private repositories is required.
        -  Click "Generate token".
    Step 4  Copy the Token:
        Make sure to copy the token immediately and store it securely. You won’t be able to see it again once you navigate away from the page.


# Cloning a repo with PAT
  ```bash
    git clone https://github.com/@<token>Digitallycamp/storedata.git
```

# What happens when the token expires ?
1.  Generate and configure your git to use new token
  -  Set the Remote URL with the New Token:
    You can update your repository’s remote URL to include the new token. Replace <new_personal_access_token> with the new token you generated, and <username> with your username
```bash
git remote set-url origin https://<username>:<new_personal_access_token>@github.com/username/repo.git
```

2. Test the New Token:

Try to push to the repository to ensure the new token is working:

```bash
git push origin main

```
