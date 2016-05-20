# Eureka!

Eventually I found that creation of a repository must be completed on the web first.

I thought it can be done by CLI only, but it was wrong.

We have to create "yet-another-repo.git" repository on github.com before executing:

    echo "# yet-another-repo" >> README.md
    git init
    git add README.md
    git commit -m "first commit"
    git remote add origin git@github.com:428desmo/yet-another-repo.git
    git push -u origin master

Otherwise, it fails as following:

    bash% git push -u origin master
    ERROR: Repository not found.
    fatal: The remote end hung up unexpectedly

