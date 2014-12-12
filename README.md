# OpenPGP Certification Policy

The OpenPGP standard ([RFC 4880](https://www.rfc-editor.org/rfc/rfc4880.txt))
allows key certifiers to label their key signatures with an URI to a policy
document that explains the conditions under which the signature was issued.

This repository publishes an exemplary certification policy document.

## Use with GnuPG
In order to add policy URI packages to key signatures made with GnuPG, one has
to add following line to the `gpg.conf`:

    cert-policy-url "https://github.com/cburkert/pgp-cert-policy/policy.txt"

In order to show policy URIs when listing key signatures, add the this to the
config:

    list-options show-policy-url

