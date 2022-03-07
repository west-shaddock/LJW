# -End-to-end encrypted messaging (E2E) is only secure if participants have a way to retrieve the correct public key for the desired recipient. 
However, to make these systems usable, users must be able to replace their keys (e.g. when they lose or reset their devices,
or reinstall their app), and we cannot assume any cryptographic means of authenticating the new keys. In the current E2E systems,
the service provider manages the directory of public keys of its registered users; 
this allows a compromised or coerced service provider to introduce their own keys and execute a man in the middle attack.
Building on the approach of CONIKS (Melara et al, USENIX Security ‘15), we formalize the notion of a Privacy-Preserving Verifiable Key Directory (VKD): 
a system which allows users to monitor the keys that the service is distributing on their behalf. We then propose a new VKD scheme which we call SEEMless,
which improves on prior work in terms of privacy and scalability. In particular, our new approach allows key changes to take effect almost immediately; 
we show experimentally that our scheme easily supports delays less than a minute, in contrast to previous work which proposes a delay of one hour.
