# Git Style Guide

* Keep your repository clean. Don’t commit big files unless they absolutely
  require git. Even in this case, prefer storing all big files in a separate
  submodule. That’s because git history can become very big and it will be pain
  for others to use the repo.
* Structure your commit message like this:

    ```
    One line summary (less than 50 characters)

    Longer description (wrap at 72 characters)
    ```

* Commit summary:
    * Less than 50 characters
    * What was changed
    * Imperative present tense (fix, add, change): ("Fix bug 123.", "Add
      'foobar' command.", "Change default timeout to 123.").
      Commits in past tense look weird to other developers e.g.
      the change ain’t happened yet and there’s question like
      “What will applying the patch do?” and you answer to this shit
      like “it will *remove utils.wrapMethod.*”.
      Also it’s
      [official git style](http://repo.or.cz/w/git.git?a=blob;f=Documentation/SubmittingPatches;hb=HEAD)
    * End with period
* Commit description:
    * Wrap at 72 characters
    * Why, explain intention and implementation approach
    * Present tense
* Commit atomicity:
    * Break up logical changes
    * Make whitespace changes separately
* Branch naming:
    * Use hyphens as word separator.
    * Use namespaces, for example,
        * `topics/topic-name` namespace every time you
          want to create a pull request and just in everyday. Use hyphens between words.
          Examples: `topics/fix-fs-utils`, `topics/add-reddit-button`.
        * `versions/x.y` namespace for supporting old versions.
          Examples: `versions/1.0`, `versions/2.1`.
