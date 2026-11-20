# Framework Consent Mode v2 & Conformité CNIL / RGPD | TAVARDT France

[![Diagnostic%20Technique](https://img.shields.io/badge/TAVARDT-Diagnostic%20Technique-5b3cf5.svg)](https://tools.tavardt.com/fr/validateur-consent-mode-v2-rgpd/)
[![Juridiction](https://img.shields.io/badge/Juridiction-France-00C853.svg)](https://ag.tavardt.com/fr/cybersecurite/)

Implémentation technique de Google Consent Mode v2, blocage préalable des traceurs et respect des lignes directrices de la CNIL et du RGPD en France.

Développé et maintenu par le pôle cybersécurité et protection des infrastructures de **[TAVARDT France](https://ag.tavardt.com/fr/)**.

---

## 1. Architecture et Ordre d'Exécution

Conformément aux recommandations de la CNIL, intégrez ce code dans le <head> avant le conteneur Google Tag Manager :

```html
<script src="consent-mode-v2.js"></script>
<!-- Google Tag Manager / measurement scripts execute here -->
```

---

## 2. Fonctionnalités Techniques Déployées

* **Refus Strict par Défaut:** ad_storage et analytics_storage initialisés en 'denied' sans traceurs résiduels.
* **Mise à Jour Pilotée par Événement:** Fonction window.tavardtConsent.update() couplée aux signaux de la CMP.
* **Anonymisation des Identifiants Publicitaires:** Activation automatique du paramètre ads_data_redaction.
* **Transmission Sécurisée Hors Traceurs:** Configuration native de url_passthrough pour les besoins de mesure agrégée.

---

## 3. Checklist de Conformité Technique

Consultez la liste des exigences techniques pour la France :

* [Checklist](https://tools.tavardt.com/fr/validateur-consent-mode-v2-rgpd/)

---

## 4. Outils de Diagnostic en Ligne (France)

Évaluez la résilience de vos applications publiques à l'aide des outils en ligne TAVARDT :

* [Validateur Consent Mode v2 et RGPD](https://tools.tavardt.com/fr/validateur-consent-mode-v2-rgpd/)
* [Analyseur d'En-têtes HTTP de Sécurité](https://tools.tavardt.com/fr/analyse-en-tetes-securite/)
* [Vérificateur DMARC et Protection de Domaine](https://tools.tavardt.com/fr/verificateur-dmarc-email/)
* [Détecteur de Fichiers Sensibles Exposés](https://tools.tavardt.com/fr/scanner-fichiers-exposes/)
* [Portail Complet d'Outils Techniques](https://tools.tavardt.com/fr/)

---

## 5. Conseil et Remédiation Technique

Pour un audit de vos conteneurs de tags et la mise en conformité CNIL de vos plateformes en France, contactez **[TAVARDT France](https://ag.tavardt.com/fr/contact/)**.
