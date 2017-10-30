# tracim_proto_jitsi
intégration with  jitsi visioconference system

Prototype simple de test, inadapté pour la production.

- Nécessite Jitsi-meet d'installé, avec token (voir https://github.com/jitsi/lib-jitsi-meet/blob/0e5d57aae5ee6e5b79a1087b7d0e0f56e60f2dba/doc/tokens.md).
C'est une fonctionnalité récente de jitsi-meet, d'ou la nécessité d'installer une version non stable du serveur XMPP prosody.
- Attention luacrypto "officiel" ne supporte pas actuellement (10-2017), OpenSSL 1.1, ce qui oblige
à forcer soit une version patché de celui-ci : https://github.com/jitsi/jitsi-meet/issues/2029 , soit de trouver une solution
pour forcer OpenSSL 1.0 .
- Integration Tracim minimale : https://github.com/inkhey/tracim/commit/ba5d6ffbf744f30cc72ddf0e7bd3806de85a1bea , configuration
dans jitsi_meet.py et videoconf.mak.
