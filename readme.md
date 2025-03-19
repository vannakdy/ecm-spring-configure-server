git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin git@github.com:vannakdy/ecm-spring-configure-server.git
git push -u origin main

git remote add origin git@github.com:vannakdy/ecm-spring-configure-server.git
git branch -M main
git push -u origin main

customer.properties
product.properties
cart.properties

# error whe push to git

    git push -u origin main
    git@github.com: Permission denied (publickey).
    fatal: Could not read from remote repository.

    Please make sure you have the correct access rights

    # Solve
        > ls -al ~/.ssh
        > sh-keygen -t rsa -b 4096 -C "dyvannak1997@gmail.com"
        > ssh-keygen -t rsa -b 4096 -C "your-email@example.com"
        > ssh-keygen -t rsa -b 4096 -C "your-email@example.com"

        > ssh-keygen -t rsa -b 4096 -C "dyvannak1997@gmail.com"
            - just enter to save it default ~/.ssh/id_rsa.
            - can set password ro enter
        > eval "$(ssh-agent -s)"
        > ssh-add --apple-use-keychain ~/.ssh/id_rsa
        > pbcopy < ~/.ssh/id_rsa.pub // get get copy in clipboard and past it to shh in your account git hup
