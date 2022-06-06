# Key

## How to (Personally) Use
1. Clone the repo `git clone https://github.com/marvinisaac/key.git`

2. Setup key for usage `cd key && ./setup`

    > Hint: 46 Wong DVD's for you

3. Confirm that it's working by checking that the following message is printed out.
    > Hi marvinisaac! You've successfully authenticated, but GitHub does not provide shell access.

## Optional Commands
- Re-create public key

    `ssh-keygen -y -f ~/.ssh/key > ~/.ssh/key.pub`

- Fit key in a single line

    ```
    cp ~/.ssh/key ~/.ssh/gpg-key && \
        echo $(tr -d '\n' < ~/.ssh/gpg-key) > ~/.ssh/gpg-key
    ```

- Encrypt a file using `key`

    `gpg --batch --passphrase-file {key location} -c {file to encrypt}`

- Decrypt a file with `key`

    `gpg --batch --passphrase-file {key location} {file to decrypt}`
