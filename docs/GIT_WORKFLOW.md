# Git and GitHub Team Workflow

## 1. Clone the shared repository

```bash
git clone https://github.com/Aneesazulfiqar23/SCD-Assignment-2.git
cd SCD-Assignment-2
```

## 2. Create a branch for your own task

Use a short name that describes the task. Examples:

```bash
git checkout -b feature/java-prototype
# or
git checkout -b docs/survey-analysis
```

## 3. Save and commit your changes

```bash
git status
git add .
git commit -m "Add <short description of actual work>"
```

Use your own Git identity and commit only work you actually completed.

## 4. Push your branch

```bash
git push -u origin feature/java-prototype
```

Replace the branch name with your actual branch.

## 5. Open a Pull Request

On GitHub, open the repository, choose **Compare & pull request**, check that the base is `main` and the compare branch is your feature branch, then create the pull request. Review the changed files before merging.

## 6. Update your local main branch

After the pull request is merged:

```bash
git checkout main
git pull origin main
```

## 7. Handle a merge conflict

If Git reports a conflict, open each conflicted file, decide which changes should remain, remove conflict markers (`<<<<<<<`, `=======`, `>>>>>>>`), then run:

```bash
git add <resolved-file>
git commit -m "Resolve merge conflict"
```

Do not claim a conflict was resolved unless one actually occurred.

## Collaboration reminders

- Each group member should use their own GitHub account and make their own commits.
- Keep `main` stable; develop work on separate branches.
- Write meaningful commit messages.
- Review a pull request before merging it.
- Do not create fake commits or attribute another person's work to yourself.
