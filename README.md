# Snapcraft PR (Pull Request)

This snap is used to test and evaluate individual pull requests for Snapcraft.
It's essentially a light wrapper around git and Python virtual environments,
simplifying a repetitive task of fetching pull requests and setting up venvs to
use them.

## How to install

    $ sudo snap install --classic snapcraft-pr

## How to use

So you have a pull request you'd like to test. When you visit the pull request,
you'll notice that each one has an ID (for example, #2120). Use that ID to fetch
the pull request and setup a virtual environment:

    $ snapcraft-pr.init <id>

Now you're ready to run that pull request's Snapcraft:

    $ snapcraft-pr <id> <typical snapcraft args>
