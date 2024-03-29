Hardening iOS
===========================================

Keeping it as simple as possible. iOS evolves fast. An old and new iPhone are underway for
further pentesting, after which these mitigations will be updated (when we have time).

.. toctree::
   :glob:
   :maxdepth: 1
   :includehidden:
   :caption: Accounts and authentication

   docs/authentication/README.md
   docs/authentication/sim-pin.md
   docs/authentication/unlock.md
   docs/authentication/password-reuse.md
   docs/authentication/passwords.md
   docs/authentication/mfa.md

.. toctree::
   :glob:
   :maxdepth: 1
   :includehidden:
   :caption: Services and applications

   docs/services/README.md
   docs/services/audit-and-block.md
   docs/services/uap.md
   docs/services/bluetooth.md
   docs/services/profiles.md
   docs/services/browsers.md
   docs/services/change-browser.md
   docs/services/messaging.md
   docs/services/email-services.md
   docs/services/ssh.md
   docs/services/vpn.md
   docs/services/tor-proxy.md
   docs/services/change-mac.md
   docs/services/edit-hosts-file.md

.. toctree::
   :glob:
   :maxdepth: 1
   :includehidden:
   :caption: Data

   docs/data/README.md
   docs/data/*

.. toctree::
   :glob:
   :maxdepth: 1
   :includehidden:
   :caption: Privacy

   docs/privacy/README.md
   docs/privacy/spam.md
   docs/privacy/search-engine.md

.. toctree::
   :glob:
   :maxdepth: 1
   :includehidden:
   :caption: Malware

   docs/malware/README.md
   docs/opsec/threats.md
   docs/malware/scanner.md
   docs/malware/clean-machine.md
   docs/malware/ransomware.md

.. toctree::
   :glob:
   :maxdepth: 1
   :includehidden:
   :caption: Operations security

   docs/opsec/README.md
   docs/opsec/threats.md
   docs/opsec/juice-jack.md
   docs/opsec/autojoin.md
   docs/opsec/email-use.md
   docs/opsec/browsing.md
   docs/opsec/ooni.md
   docs/opsec/*

.. toctree::
   :glob:
   :maxdepth: 1
   :includehidden:
   :caption: Guards! Guards!

   docs/guards/README.md
   docs/guards/lockdown.md
