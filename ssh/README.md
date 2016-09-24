## Info

Follow instructions [here](https://stribika.github.io/2015/01/04/secure-secure-shell.html).

You can recompile OpenSSH to the newest version and user supervisord to manage its execution (uninstalling the package-maintained version). However, this makes installing updates and security fixes tedious, but removes the Host name string from the configuration response on initial connect. You can link it with LibreSSL which may be more secure.

## Key generation

`ssh-keygen -t ed25519 -o -a 100`

and use a strong password. The `-a 100` tells it to iterate the hash function 100 times. Using values like this or larger makes brute-force password cracking more cumbersome.
