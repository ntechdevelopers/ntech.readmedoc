Git Conventions
===================================

**Git flow**

# Commit message

When writing a commit message, it should adhere to the following guidelines:

**General Rules**

* The subject of the commit message is limited to 50 characters
* Capitalize the first letter of the subject
* Do not end the subject with a period
* Use an imperative style in the subject (`Add password validation` vs `Added password validation`)
* Add a commit body when additional background for the commit is necessary
* Body is separated from subject by one blank line

**Semantic Subjects**

Commit messages' subjects are preceded by a tag to make it easier to read through them and filter them out:

```
<type>: <commit subject>
```

For example:

```
feat: Add password validation
```

Tags:

* `feat`: New feature or functionality for the user, not a new feature for the build script
* `fix`: Bug fix for the user, not a fix to a build script
* `docs`: Changes to the documentation
* `style`: Formatting, missing semi-colons, etc; no production code change
* `refactor`: Code refactoring (variable renaming or code restructuring) that doesn't affect the functionality
* `test`: Adding, fixing, or refactoring tests; no production code change
* `chore`: Updating build scripts or upgrading dependencies; no production code change
* `misc`: Use for anything that doesn't clearly fall into any of the previous categories

# Branch name

Example:

```
features/001_login_logout
```