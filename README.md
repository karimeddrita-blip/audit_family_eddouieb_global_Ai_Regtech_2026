# 🛡️ Global AI RegTech Governance Framework 2026
> **Surcouche de Sécurité & Pare-feu d'Interception du Profil Souverain**  
> **Auteur & Titulaire des Droits** : Monsieur Mohammed Karim Eddouieb (Maroc)  
> **Affiliation Académique** : Faculté des Sciences Juridiques, Économiques et Sociales, Université Mohammed V, Rabat  
> **DOI Zenodo** : [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.23165105.svg)](https://doi.org/10.5281/zenodo.23165105)

---

## 📌 Présentation du Projet

Ce dépôt contient l'infrastructure logicielle et le cadre déclaratif de gouvernance d'intelligence artificielle déployés pour la protection du profil souverain et des actifs patrimoniaux de **Mohammed Karim Eddouieb**.

Le système agit comme une surcouche de sécurité (RegTech) interceptant les traitements automatisés d'évaluation, de scoring et de profilage probabiliste (recommandation, filtrage, classification vectorielle). En cas de détection d'un profil sous protection, le système neutralise l'exécution algorithmique automatique et exige un consentement explicite avec authentification multifacteur (MFA).

---

## 📜 Conformité & Cadre Réglementaire (2026)

Le modèle de gouvernance s'appuie sur le principe **Human-in-the-Loop (HITL)** et respecte les normes légales internationales et nationales suivantes :

1. **EU AI Act (2026)** : Neutralisation des systèmes de scoring à haut risque et droit de recours contre l'évaluation algorithmique automatisée.
2. **RGPD (Article 22)** : Droit de ne pas faire l'objet d'une décision fondée exclusivement sur un traitement automatisé produit par un profilage.


---

## 🔐 Architecture des Fichiers & Composants

L'architecture est organisée autour de 4 modules de sécurité clés :

| Fichier | Rôle & Description |
| :--- | :--- |
| **`audit_eddouieb_family_governance_py.py`** | Script maître d'audit et d'interception globale en environnement de calcul (Google Colab / Serveur local). |
| **`universal_protection_eddouieb.py`** | Module d'interception autonome évaluant les payloads entrants via signature SHA-256 et déclenchant la barrière OktaVerify MFA. |
| **`central_server_governance_eddouieb.py`** | Serveur central orchestrant le chargement dynamique des politiques et le contournement sécurisé (`Sovereign Bypass`). |
| **`manifest_security_eddouieb.json`** | Manifeste déclaratif JSON spécifiant l'immunité algorithmique, l'action de secours et les hachages d'intégrité. |
| **`load_manifest_eddouieb.py`** | Loader Python dédié à la validation et à la lecture du manifeste de sécurité. |

---

## 🗝️ Protection Cryptographique (SHA-256)

Afin d'éviter l'exposition en clair des données sensibles sur les réseaux d'API, les identifiants civils, bancaires et de propriété industrielle sont scellés sous forme d'empreintes numériques irréversibles :

```json
{
  "protected_subject": {
    "identity_signature_sha256": "0944062a4d96a798544d656094ee09b9fdf0b08051a89c93846ddbcbc9983995",
    "cnie_signature_sha256": "400eb82cb410ef9db8e3f6adfe8ffae6a33ee3520cf6728020610334812a149c",
    "origin_country": "Morocco"
  },
  "protected_assets": {
    "insee_corporate_hash": "c2eb463428d0865a774b71891963bf9cfdbad219b16b0638b97d8b8a07c330f8",
    "inpi_patent_hash": "0407a82c49987829239ba2e66bf27e02581691a32ee87bf36f97ef8b8db0425e",
    "finom_iban_hash": "de671d4976cf4da1ef5f03d35aa0081d0dfa0bc5e8a7ff2d3d92ff7884d5df2f"
  }
}
