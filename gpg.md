---
layout: page
title: GPG and identity
permalink: /gpg/
---

I use GPG to sign my email and to prove online identity on some website. You can use my public key to verify it's me and to encrypt messages if you want.

- The fingerprint of my public key is `17218f250c9ab128a04b29591131bb2904f15681`
- You can retrieve the key on [keys.openpgp.org](https://keys.openpgp.org/search?q=17218f250c9ab128a04b29591131bb2904f15681).
- [Keyoxide](https://keyoxide.org/francois.orieux@universite-paris-saclay.fr)
  make the link between my key and online identity, that are
  - this domain `orieux.fr`
  - the github account [forieux](https://github.com/forieux)
- The Keyoxide profile also works with the
  [fingerprint](https://keyoxide.org/17218f250c9ab128a04b29591131bb2904f15681).

What's it means ? Not that much. If you receive an email from <francois.orieux@universite-paris-saclay.fr> signed with the key, it means that the person who sends this email has access to the secret key, control the claims (via the key) and proofs (via the github account for instance) mentioned on the Keyoxide profile. The server `keys.openpgp.org` also verify that the email is valid, not necessarily that it's me that read the verification email. However, to sign, decrypt or make a claim, the person needs access to the password protected local secret key. So the bad person must have my secret key (that I keep local) and my password. Proofs are also password protected, at least, since a login (to github) is necessary.
