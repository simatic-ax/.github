# Fork & Pull Request Process

This document outlines clearly how you can contribute code improvements or feature proposals using GitHub's standard fork and pull request mechanism.

## Overview

A fork allows you to freely experiment with changes without affecting the original repository. When your changes are ready, you submit them back as a **pull request (PR)**. The repository maintainers will review your changes and merge them if they are beneficial.

## Step-by-Step Guide

1. **Fork the Repository**
   - Navigate to the repository on GitHub and click the **Fork** button.
   - GitHub will create a copy under your own account.

2. **Clone Your Fork**
   - Clone your fork locally, replacing `your-username` and `repository-name`:
   ```bash
   git clone https://github.com/your-username/repository-name.git
   ```

3. **Create a Development Branch**
   - Always use separate branches for new features or fixes:
   ```bash
   git checkout -b feature/my-new-feature
   ```
   - Using separate branches isolates your changes from the main development line, making collaboration easier and cleaner.

4. **Make Your Changes**
   - Implement the changes or improvements you've planned. Ensure your code conforms to coding standards and style guides.
   - Commit your changes clearly and descriptively:
   ```bash
   git add .
   git commit -m "Add a clear description of your changes"

5. **Push Your Changes**
   - After committing your changes locally, push your branch back up to your forked repository on GitHub:
   ```bash
   git push origin feature/my-new-feature

6. **Open a Pull Request**
   - Visit your forked repository on GitHub and click the green button labeled Compare & pull request.
   - Clearly describe your changes. Explain the purpose, any implications, and include supporting details that may assist maintainers in reviewing your contribution.

7. **Review and Integration**
   - Maintainters will carefully review your Pull Request (PR).
      - If questions or modifications are required, maintainers will communicate these directly within the PR.
      - Respond to feedback accordingly and commit additional changes if requested.
   - Once maintainers approve, they will merge your PR into the main branch of the original repository.


## Knowlegde Base

1. **Create a fork**
   - [Fork a repsitory](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/working-with-forks/fork-a-repo)
2. **Sync a fork**
   - [Syncing a fork](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/working-with-forks/syncing-a-fork)
3. **Create a PR from a fork**
   - [Creating a pull request from a fork](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request-from-a-fork)