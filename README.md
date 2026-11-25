# Framework Consent Mode v2 & Conformité CNIL / RGPD

[![Diagnostic Technique](https://img.shields.io/badge/TAVARDT-Diagnostic%20Technique-5b3cf5.svg)](https://tools.tavardt.com/fr/validateur-consent-mode-v2-rgpd/)
[![JavaScript](https://img.shields.io/badge/JavaScript-Node.js-yellow.svg)](https://nodejs.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

Implémentation technique de Google Consent Mode v2, blocage préalable des traceurs et respect des lignes directrices de la CNIL et du RGPD en France.

***

## 1. Architecture et Ordre d'Exécution

Conformément aux recommandations de la CNIL, intégrez ce code dans le <head> avant le conteneur Google Tag Manager :

```html
<script src="consent-mode-v2.js"></script>
<!- Google Tag Manager / measurement scripts execute here ->
```

***

## 2. Fonctionnalités Techniques Déployées

* **Refus Strict par Défaut:** ad_storage et analytics_storage initialisés en 'denied' sans traceurs résiduels.
* **Mise à Jour Pilotée par Événement:** Fonction window.tavardtConsent.update() couplée aux signaux de la CMP.
* **Anonymisation des Identifiants Publicitaires:** Activation automatique du paramètre ads_data_redaction.
* **Transmission Sécurisée Hors Traceurs:** Configuration native de url_passthrough pour les besoins de mesure agrégée.

***

## 3. Checklist de Conformité Technique

Consultez la liste des exigences techniques pour la France :

* Checklist

***

## 4. Outils de Diagnostic en Ligne (France)

Évaluez la résilience de vos applications publiques à l'aide des outils en ligne TAVARDT :

* [Analyseur d'En-têtes HTTP de Sécurité](https://tools.tavardt.com/fr/analyse-en-tetes-securite/)
* [Vérificateur DMARC et Protection de Domaine](https://tools.tavardt.com/fr/verificateur-dmarc-email/)
* [Détecteur de Fichiers Sensibles Exposés](https://tools.tavardt.com/fr/scanner-fichiers-exposes/)
* [Portail Complet d'Outils Techniques](https://tools.tavardt.com/fr/)

***

## 5. Conseil et Remédiation Technique

Pour un audit de vos conteneurs de tags et la mise en conformité CNIL de vos plateformes en France, contactez **TAVARDT**.

***

## Liens Utiles

* **Portail Entreprise:** https://ag.tavardt.com/fr/
* **Suite de Diagnostic:** https://tools.tavardt.com/fr/
* **Contact Technique:** https://ag.tavardt.com/fr/contact/

***

### Licence
Distribué sous la licence MIT.

***

© 2026 TAVARDT. Tous droits réservés.
