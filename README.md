# Minor edits

Use githubs online editing facilities to change any of

* https://github.com/polysensus/polysensus.github.io/blob/main/content/benefits/benefit-1.md
* https://github.com/polysensus/polysensus.github.io/blob/main/content/benefits/benefit-2.md
* https://github.com/polysensus/polysensus.github.io/blob/main/content/benefits/benefit-3.md

The tagline and socials can be modified by editing the config:

* https://github.com/polysensus/polysensus.github.io/blob/main/config.yaml

The theme index page can also be edited, but more care is required

* https://github.com/polysensus/polysensus.github.io/blob/main/themes/hugo-theme-lean-launch-page/layouts/index.html

# Major edits

To make these it is more efficient and safe to setup local tooling so that the
changes can be previewed

## Pre-requisites

The minimum list of command line tools required before attempting this is:

* brew (mac or linux)

  `/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"`

  https://brew.sh/

* git (mac) there are a couple of options:
  * Run `brew install git`
  * Open a terminal and run git. it should prompt you to install the XCode commandline tools.
  See https://git-scm.com/book/en/v2/Getting-Started-Installing-Git

* hugo (the site builder)

  `brew install hugo`

* go-task (automation tool used to conveniences specific to this website repository)

  `brew install go-task/tap/go-task`

  See https://taskfile.dev/installation/

## Editing

1. Choose a directory to work in

  `mkdir ~/polysensus`
  `cd ~/polysensus`

2. Clone the repository `git clone git@github.com:polysensus/polysensus.github.io.git`

3. `cd ~/polysensus/polysensus.github.io`

4. task build

5. task serve

6. Visit http://localhost:1313/

7. Edit any if the files listed in "Minor edits" (leaving task serve running)

8. Your site should re-build

9. Push your changes
   a. git add .
   b. git commit -m "short description of changes"
   c. git push

10. Visit https://github.com/polysensus/polysensus.github.io

If you locate the actions menu just below the repo title, you will be able to
watch the progress of the site deployment



