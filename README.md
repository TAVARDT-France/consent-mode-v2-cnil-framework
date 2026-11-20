# Cadre Technique Consent Mode v2 & Lignes Directrices CNIL | TAVARDT France

[![Validador de Consentimento](https://img.shields.io/badge/TAVARDT-Diagn%C3%B3stico%20T%C3%A9cnico-5b3cf5.svg)](https://tools.tavardt.com/fr/validateur-consent-mode-v2-rgpd/)
[![Conformidade](https://img.shields.io/badge/Jurisdi%C3%A7%C3%A3o-France-00C853.svg)](https://ag.tavardt.com/fr/cybersecurite/)

Implémentation technique de Google Consent Mode v2, blocage des traceurs non essentiels et conformité aux lignes directrices de la CNIL et du RGPD en France.

Desenvolvido e mantido pela divisão de privacidade digital e engenharia de dados da **[TAVARDT France](https://ag.tavardt.com/fr/)**.

---

## 1. Architecture et Ordre d'Exécution

Conformément aux exigences de la CNIL, ce fichier doit être inséré dans la section <head> de votre site web immédiatement avant le conteneur Google Tag Manager :

```html
<script src="consent-mode-v2.js"></script>
<!-- O contentor do Google Tag Manager ou scripts de medição seguem aqui -->
```

---

## 2. Fonctionnalités Techniques Déployées

* **Refus et Blocage par Défaut:** Configure ad_storage, analytics_storage et ad_user_data sur 'denied' dès la première seconde de chargement.
* **Mise à Jour Événementielle du Consentement:** Expose la fonction window.tavardtUpdateConsent() émettant l'événement tavardt_consent_updated dans le dataLayer.
* **Caviardage des Identifiants Publicitaires:** Active ads_data_redaction pour supprimer les identifiants de clic en l'absence de consentement.
* **Liaison Interdomaines Sécurisée:** Configure url_passthrough pour préserver l'attribution sans déposer de cookies illicites.

---

## 3. Checklist de Conformité Technique

Consulte a lista detalhada de requisitos técnicos para este país:

* [Checklist Técnico de Conformidade](checklist.md)

---

## 4. Outils de Diagnostic en Ligne (France)

Audite a conformidade das suas etiquetas e proteja o seu domínio com ferramentas online verificadas:

* [Validateur Consent Mode v2 et RGPD](https://tools.tavardt.com/fr/validateur-consent-mode-v2-rgpd/)
* [Analyseur d'En-têtes HTTP de Sécurité](https://tools.tavardt.com/fr/analyse-en-tetes-securite/)
* [Vérificateur DMARC et Protection de Domaine](https://tools.tavardt.com/fr/verificateur-dmarc-email/)
* [Détecteur de Fichiers Sensibles Exposés](https://tools.tavardt.com/fr/scanner-fichiers-exposes/)
* [Portail Complet d'Outils Techniques](https://tools.tavardt.com/fr/)

---

## 5. Conseil et Gouvernance des Balises

Pour des audits de conformité CNIL, la sécurisation de vos conteneurs GTM et l'optimisation de vos mesures en France, contactez **[TAVARDT France](https://ag.tavardt.com/fr/contact/)**.
