# Configuration

A guide to configuring git and connecting to GitHub on the command line.

## Step 1: Set Your Identity

First, set your identity in git so that your commits have author information attached. Enter the following two commands to set your name and email:

```bash
git config --global user.name "Your Name"
git config --global user.email username@email.com
```

## Step 2: Check for Existing SSH Keys

It's advised you set up an SSH key to authenticate with GitHub. If you don't do this you'll have to enter your username and password every time.

First, check for existing SSH keys on your computer by showing the contents of the `.ssh` directory in your home folder.

```bash
ls ~/.ssh
```

If you already see an `id_rsa` and `id_rsa.pub`, you have already created a key pair. If you know you created these, you can skip to Step 4. If you're unsure, you should delete these and generate a new key. Delete with `rm id_rsa*`.

If your `.ssh` folder does not contain keys (or you deleted them) or the folder does not exist (you'll see `ls: cannot access .ssh: No such file or directory`), proceed to step 3.

## Step 3: Generate SSH keys

Use the `ssh-keygen` command to generate a new SSH key:

```
ssh-keygen -t rsa -C "username@computer"
```

Be sure to identify the key with a descriptive name in the comment (`-C`) so you know which computer it belongs to. For example `bob@raspberrypi` or `frank@laptop`.

You'll see the following:

```
Generating public/private rsa key pair.
# Enter file in which to save the key (/home/you/.ssh/id_rsa):
```

Hit `Enter` to save the key to the default location.

Next, you'll be prompted to enter a passphrase. Type this in and hit `Enter` or just Hit `Enter` to leave blank.

Then add your new key to the `ssh-agent`:

```bash
ssh-add ~/.ssh/id_rsa
```

Now you'll find `id_rsa` and `id_rsa.pub` files in your `.ssh` directory. These are your public and private RSA keys. Never share your private key.

## Step 4: Add your SSH key to GitHub

Reveal the contents of your public key:

```bash
cat ~/.ssh/id_rsa.pub
```

You will paste your public key in to GitHub which will validate against your private key.

Sign in to [github.com](https://github.com/), go to your [Account Settings](https://github.com/settings/admin) and go to [SSH Keys](https://github.com/settings/ssh) in the left sidebar.

Click `Add SSH Key` and enter a title to describe which computer the key belongs to, e.g. "Raspberry Pi" or "Ubuntu Laptop".

Now paste the whole public key in to the key field and click the `Add key` button.

Return to the command line and test your SSH connection to GitHub:

```bash
ssh -T git@github.com
```

If you have any issues, see [GitHub's help page](https://help.github.com/articles/generating-ssh-keys#step-4-test-everything-out)

Now proceed to [Using Git Guide](git.md).
