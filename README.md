# ubuntu-install-Tor-Relay-update-tor-relay-version


==========================================================================================

Nickname    myRelay  # Change "myRelay" to something you like
ContactInfo your@e-mail  # Write your e-mail and be aware it will be published
ORPort      9001          # You might use a different port, should you want to
DirPort 9030
ExitRelay   0
SocksPort   0

ControlPort 9051
CookieAuthentication 1
CookieAuthFileGroupReadable 1

==========================================================================================

deb     [arch=<ARCHITECTURE> signed-by=/usr/share/keyrings/tor-archive-keyring.gpg] https://deb.torproject.org/torproject.org focal main
deb-src [arch=<ARCHITECTURE> signed-by=/usr/share/keyrings/tor-archive-keyring.gpg] https://deb.torproject.org/torproject.org focal main

==========================================================================================

wget -qO- https://deb.torproject.org/torproject.org/A3C4F0F979CAA22CDBA8F512EE8CBC9E886DDD89.asc | gpg --dearmor | tee /usr/share/keyrings/tor-archive-keyring.gpg >/dev/null

