# Drupal modudle to include an html list of publications from Hal directly in your website #

## How does it works ? ##

This plugin creates a new filter which can be activated or not.

Once installed, create a new node and put on the body this modele:

`{{webpage_from_hal|url=http://hal.univ-grenoble-alpes.fr/Public/afficheRequetePubli.php?auteur_exp=boris,morel&CB_auteur=oui&CB_titre=oui&CB_article=oui&langue=Francais&tri_exp=annee_publi&tri_exp2=typdoc&tri_exp3=date_publi&ordre_aff=TA&Fen=Aff&css=../css/VisuRubriqueEncadre.css}}`

By this filter, Drupal get the url and include the html content directly on your body.

## Install ##
  1. This module require [saga_base](https://github.com/Saga-UGA/saga_base) module.
  1. To install both plugins, refer to the official [Drupal documentation](https://drupal.org/node/895232).

## Activate ##
  1. The Drupal filter are managed on `text formats` section (/admin/config/content/formats).
  1. Choose which text format uses this filter.
  1. Enable `Include html content from hal url` filter.

**Note:**
> Caution, this filter need to be in the first. If an other filter alter html content, there is a good chance that this filter can't retrieve the good syntaxe. So do not work !  
  
## Support ##

GitHub is the good way to contribute on this project.
  - Issue
  - Pull request
  - [...]
