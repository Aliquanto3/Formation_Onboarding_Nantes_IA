# 🎓 Formation Onboarding IA – Nantes

Bienvenue ! Ce dépôt contient le matériel pédagogique de la session « Comprendre l’IA par la pratique » (1 h 30) animée chez Wavestone Nantes.

[![Launch Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/Aliquanto3/Formation_Onboarding_Nantes_IA/HEAD?labpath=IA_HandsOn_Demo_v2.ipynb)

---

## Sommaire
1. [Objectifs](#objectifs)
2. [Prérequis](#prérequis)
3. [Démarrage instantané (MyBinder)](#démarrage-instantané-mybinder)
4. [Exécution locale](#exécution-locale)
5. [Contenu du dépôt](#contenu-du-dépôt)
6. [FAQ](#faq)
7. [Licence](#licence)

---

## Objectifs

- **Découvrir** les grands types d’IA (classification, réseaux de neurones, génération de texte).  
- **Manipuler** un notebook Python commenté, sans pré-requis en programmation.  
- **Appréhender** les limites : biais, sécurité, gouvernance.  

---

## Prérequis

Aucun logiciel à installer si vous utilisez le lien MyBinder.  
Pour un lancement **local**, vous aurez besoin de :

- Python ≥ 3.9 (recommandé : 3.11)
- `pip` à jour : `python -m pip install --upgrade pip`
- Windows : activer les “long paths” ou utiliser un environnement virtuel court (voir FAQ).

---

## Démarrage instantané (MyBinder)

1. Cliquez sur le badge **Launch Binder** en haut de ce fichier.  
2. Patientez ~30 s (premier build) puis le notebook `IA_HandsOn_Demo_v2.ipynb` s’ouvre.  
3. Dans le menu **Run ▸ Run All** (*Exécuter ▸ Exécuter tout*).  
4. Manipulez ! Les changements ne sont pas conservés : chaque participant a sa propre session.

> *Astuce :* ouvrez le lien une fois avant la formation pour pré-chauffer l’image Docker ; les lancements suivants seront quasi instantanés.

---

## Exécution locale

```bash
# 1. Clonez le dépôt
git clone https://github.com/Aliquanto3/Formation_Onboarding_Nantes_IA.git
cd Formation_Onboarding_Nantes_IA

# 2. Créez un environnement virtuel court (évite l’erreur de chemin sous Windows)
python -m venv .venv
.\.venv\Scripts\activate      # PowerShell
# source .venv/bin/activate   # macOS / Linux

# 3. Installez les dépendances
pip install --upgrade pip
pip install -r requirements.txt ipykernel

# 4. Lancez VS Code et sélectionnez l’interpréteur .venv
code .

# 5. Ouvrez IA_HandsOn_Demo_v2.ipynb, puis ▶ Exécuter tout
