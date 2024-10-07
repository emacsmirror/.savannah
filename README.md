# Mirrors of GNU Emacs, GNU ELPA and NonGNU ELPA

This repository contains the tooling used to mirror these three repositories
from [Savannah](https://savannah.gnu.org) to GitHub.

|                 | Upstream Repository                                | Mirror Repository                                                     |
| --------------- | -------------------------------------------------- | --------------------------------------------------------------------- |
| **GNU Emacs**   | https://git.savannah.gnu.org/cgit/emacs.git        | [emacsmirror/emacs](https://github.com/emacsmirror/emacs)             |
| **GNU ELPA**    | https://git.savannah.gnu.org/cgit/emacs/elpa.git   | [emacsmirror/gnu_elpa](https://github.com/emacsmirror/gnu_elpa)       |
| **NonGNU ELPA** | https://git.savannah.gnu.org/cgit/emacs/nongnu.git | [emacsmirror/nongnu_elpa](https://github.com/emacsmirror/nongnu_elpa) |

Savannah has a [project](https://savannah.gnu.org/projects/emacs/) and a
[usage](https://savannah.gnu.org/git/?group=emacs) page for this group of
repositories.

> [!NOTE]
> These mirrors are updated hourly.

> [!IMPORTANT]
> Not all branches are included in these mirrors.
>
> Note in particular that NonGNU ELPA's `elpa/coffee-mode`
> branch is omitted because it is corrupted,
> see [defunkt/coffee-mode#367](https://github.com/defunkt/coffee-mode/issues/367)
> and [debbugs#2365241](https://debbugs.gnu.org/cgi/bugreport.cgi?bug=bug%2365241).
>
> The following refspecs are used:

- GNU Emacs

  ```
  +refs/heads/emacs-*:refs/heads/emacs-*
  +refs/tags/emacs-1*:refs/tags/emacs-1*
  +refs/tags/emacs-2*:refs/tags/emacs-2*
  +refs/tags/emacs-3*:refs/tags/emacs-3*
  ```

- GNU ELPA

  ```
  +refs/heads/main:refs/heads/main
  +refs/heads/elpa-admin:refs/heads/elpa-admin
  +refs/heads/externals-release/*:refs/heads/externals-release/*
  +refs/heads/externals/*:refs/heads/externals/*
  ```

- NonGNU ELPA

  ```
  +refs/heads/main:refs/heads/main
  +refs/heads/elpa-release/*:refs/heads/elpa-release/*
  +refs/heads/elpa/*:refs/heads/elpa/*
  ^refs/heads/elpa/coffee-mode
  ```
