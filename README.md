# Key

## How to Use
1. Clone the repo

    `git clone https://github.com/marvinisaac/key.git`

2. Decrypt key

    `gpg key.gpg`

    > Hint: 46 Wong DVD's for you

3. Copy created `key` file to SSH folder

    `cp key ~/.ssh`

4. Set proper permissions

    `chmod 700 ~/.ssh/key`

5. Copy and customize SSH config 

    `cp config ~/.ssh`

6. Verify that it is working

    `ssh -T github.com`
