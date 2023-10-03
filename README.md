# Estimation du Coup du Certificat d'Immatriculation

Ceci est une version modifiée et réduite du simulateur de coût du certificat d'immatriculation de l'ANTS sur le site [service-public.fr/simulateur/calcul/cout-certificat-immatriculation](https://www.service-public.fr/simulateur/calcul/cout-certificat-immatriculation).

Elle comprend les véhicules pris en charge pour de l'import automobile Français et utilise la même erreur de 10% que le simulateur original.

Pour des raisons de litiges passés, les fichiers sont compilés en dehors des données officielles du gouvernement disponibles sur leur dépôt Gitlab : [gitlab.com/pidila/sp-simulateurs-data/](https://gitlab.com/pidila/sp-simulateurs-data/-/tree/master).

> [!NOTE]
> Les données gouvernementales sont mises à jour parfois sans que le fichier qu'ils fournissent ne soit lui-même mis à jour. Afin d'être au plus proche de la réalité, les données utilisées par ce simulateur sont mises à jour régulièrement dans `data.json`.

Si vous souhaitez utiliser ce simulateur, vous pouvez le faire, au risque de ne pas pouvoir modifier les données pour ajouter des éléments supplémentaires.

## Usage

Ce simulateur est une série de modules pouvant être appelés dans n'importe quel fichier comme ceci :

### HTML

```html
<script type="module">
    import Simulator from './path/to/Simulator.js';
</script>
```

### JavaScript

```javascript
import Simulator from './path/to/Simulator.js';
```

## Limitations

Ce simulateur ne prend en charge que les choix suivants :
- Véhicule de tourisme (VT ou M1) ex-Voiture particulière (VP)
- Camionnette, Utilitaire pour le transport de marchandises jusqu'à 3,5 tonnes (CTTE, N1)
- Camping-car et autre véhicule VASP d'un poids maximal inférieur ou égal à 3,5 tonnes

Il n'est possible de faire des calculs pour des véhicules Importés en France ayant déjà été immatriculés à l'étranger.

## Avertissement relatif à la créativité du projet

> [!WARNING]
> Ce projet est une création personnelle effectuée en dehors de toute structure et pouvant être amené à être proposé à l'utilisation. Il n'est, en aucun cas, lié à l'ANTS ou à l'administration Française.
>
> Les éléments de ce projet ne sont la propriété légale d'aucune entité et peut être vu comme un petit projet personnel.
>
> Le développement du projet a démarré le 13/06/2023, la base de développement n'est pas et ne sera pas rendue publique.
>
> Ce projet est identifié par une clé GPG personnelle identifiée par l'empreinte suivante :
> - `F2D67BFDF7AD74EE` (4096R)
