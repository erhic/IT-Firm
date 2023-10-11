> Any line of the commit message cannot be longer 100 characters!<br/>
> This allows the message to be easier to read on GitHub as well as in various Git tools.

##### Type

Must be one of the following:

- **feat**: A new feature
- **fix**: A bug fix
- **docs**: Documentation only changes
- **style**: Changes that do not affect the meaning of the code (white-space, formatting, missing
  semi-colons, etc)
- **refactor**: A code change that neither fixes a bug nor adds a feature
- **perf**: A code change that improves performance
- **test**: Adding missing tests
- **chore**: Changes to the auxiliary tools such as release scripts
- **build**: Changes to the dependencies, devDependencies, or build tooling
- **ci**: Changes to our Continuous Integration configuration

##### Scope

The scope could be anything that helps specify the scope (or feature) that is changing.

Examples

- fix(select):
- docs(menu):

##### Subject

The subject contains a succinct description of the change: [you can add Git Emojis if you want here](https://gitmoji.dev/)

- use the imperative, present tense: "change" not "changed" nor "changes"
- don't capitalize first letter
- no period (.) at the end

##### Body

Just as in the **subject**, use the imperative, present tense: "change" not "changed" nor "changes".
The body should include the motivation for the change and contrast this with previous behavior.

##### Footer

The footer should contain any information about **Breaking Changes** and is also the place to
reference GitHub issues that this commit **Closes**, **Fixes**, or **Relates to**.

> We highlight Breaking Changes in the ChangeLog. These are as changes that will require
> community users to modify their code after updating to a version that contains this commit.

##### Sample Commit messages

```markdown
fix(autocomplete): don't show the menu panel when readonly

- this could sometimes happen when no value was selected

Fixes #11231
```

```text
feat(chips): trigger ng-change on chip addition/removal

- add test of `ng-change` for `md-chips`
- add docs regarding `ng-change` for `md-chips` and `md-contact-chips`
- add demo for ng-change on `md-chips`
- add demo for ng-change on `md-contact-chips`

Fixes #11161 Fixes #3857
```

````text
refactor(content): prefix mdContent scroll- attributes

    BREAKING CHANGE: md-content's `scroll-` attributes are now prefixed with `md-`.

    Change your code from this:
    ```html
    <md-content scroll-x scroll-y scroll-xy>
    ```

    To this:
    ```html
    <md-content md-scroll-x md-scroll-y md-scroll-xy>
    ```
````

<br/>
