# Sys

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
