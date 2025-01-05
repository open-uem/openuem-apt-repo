# OpenUEM Debian/Ubuntu repository

Repository containing the GPG public key and instructions to add the Debian/Ubuntu repository

To download the public GPG key:

`curl -fsSL https://apt.openuem.eu/pgp-key.public | sudo gpg --dearmor -o /usr/share/keyrings/openuem.gpg`

To add the repository:

`echo "deb [arch=amd64 signed-by=/usr/share/keyrings/openuem.gpg] https://apt.openuem.eu stable main" | sudo tee /etc/apt/sources.list.d/openuem.list`

Reference: https://earthly.dev/blog/creating-and-hosting-your-own-deb-packages-and-apt-repo/#step-2-creating-an-apt-repository
