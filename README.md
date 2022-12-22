# sys

This is to easily retrieve my debian system with all of its settings.

For some installations user is not in sudoers by default.
If this is the then case run the following lines (remember
to replace arguments in < > for the relevant ones):

```bash
su
usermod -aG sudo <username>
exit
sudo whoami
```

The last line should output `root` if you have sudo rights.

After setting your user as a sudoer you can run the following lines:

```bash
sudo apt install git -y
cd
git init
git remote add origin git@github.com:f1lem0n/sys.git
git pull
```

**CAUTION:** only run `retrieve-sys` on a new system, this script
makes changes to the filesystem and may result in files corruption!
