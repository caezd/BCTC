---
icon: circle-info
---

# Informations d'appel

<div align="center"><figure><img src="../../.gitbook/assets/Information_appel.jpg" alt=""><figcaption></figcaption></figure></div>

1. **Date/heure Demande :** La date et l'heure de la demande (lorsque le téléphoniste décroche le téléphone) OU la date et l'heure planifiée s'il s'agit d'une [réservation](../../9.-reservations.md).
2. **Date/heure reçu :** La date et l'heure de la création de l'appel (avec la touche <kbd>**F6**</kbd>).
3. **Date/heure donnée :** La date et l'heure à laquelle l'appel a été accepté dans une tablette.
4. **Date/heure chez client :** La date et l'heure à laquelle le taxi indique (à l'aide d'un bouton dans sa tablette) qu'il est arrivé devant l'adresse du client.
5. **Date/heure client à bord :** La date et l'heure à laquelle le client embarque dans le véhicule (via le bouton Emb. ou grâce au démarrage du compteur virtuel).
6. **Date/heure terminée :** La date et l'heure à laquelle le chauffeur a indiqué(à l'aide d'un bouton dans sa tablette) que l'appel était terminé.
7. **Appel ID :** Chaque appel possède un numéro d'identification unique. Il est possible de rechercher un appel en inscrivant ce numéro dans le champ "Remarque" lors d'une [recherche complète](recherche-dappels.md), sous la forme `ID:1234`.
8. **Téléphoniste :** Nom de l'employé qui a créé l'appel (en appuyant sur <kbd>**F6**</kbd> pour l'envoyer dans le système).
9. **Répartiteur :** Nom de l'employé qui a distrubé l'appel dans un véhicule. Si l'appel était en `répartition automatique`, il sera indiqué. <mark style="background-color:yellow;">À moins d'une exception nécessitant une manipulation spécifique de la part d'un opérateur, il ne devrait y avoir aucun nom dans cette case !</mark>
10. **Zonage :** La zone principale de l'adresse ainsi que ses dessertes.
11. **# Voiture :** La voiture qui a desservi l'appel.
12. **Zone :** La zone dans laquelle l'appel a été distrubé dans la tablette.
13. **Remarque :** La remarque peut être inscrite par le téléphoniste, des restrictions cochéea, le nom d'un commerce (selon les raccourcis d'adresse) ou le commentaire inscrit dans un tronçon du zonage.
14. **Options spéciales :**&#x20;
    * Répartition manuelle : si coché, cet appel a été réparti manuellement.
    * Marquer pour identifier : si coché, cet appel a été marqué pour être identifié ultérieurement (suivi).
    * Appel prioritaire : les appels prioritaires sont des appels qui sont répartis avant les appels réguliers (e.g. les réservations, numéros d'ordre). Dans la liste des appels en attente, il sont surlignés en vert.
15. **Type Véhicule :** Le type de véhicule demandé par le client. Si les trois sont cochés, tous les véhicules se qualifient pour cet appel. Permet également de spécifier le nombre de clients au besoin.
16. **Options :**&#x20;
    * Sauvegarder : Permet de sauvegarder toutes modifications apportées à un appel qui n'est pas encore réparti, comme la remarque ou l'heure demandée. <mark style="background-color:yellow;">Si vous changez l'heure d'une réservation de cette façon, pensée à modifier l'heure dans</mark> <mark style="background-color:yellow;"></mark><mark style="background-color:yellow;">`Date/heure Demande`</mark> <mark style="background-color:yellow;"></mark><mark style="background-color:yellow;">et dans</mark> <mark style="background-color:yellow;"></mark><mark style="background-color:yellow;">`Remarque`</mark><mark style="background-color:yellow;">.</mark>
    * Effacer : Permet d'effacer un appel n'était pas encore réparti.
    * Reprise : Permet de reprendre un appel réparti dans une tablette.
    * Envoyer maintenant : Permet d'envoyer sur-le-champs un appel prévu pour une date/heure ultérieure.
    * Ouvrir module : Permet d'ouvrir les informations de paiement d'un Numéro d'ordre lorsque l'appel est complété. Il est également possible pour un opérateur ou un chef d'équipe d'ajuster un montant en cas de besoin.\
      ![](<../../.gitbook/assets/image (23).png>)
    * Voir trace GPS : Lorsqu'un appel est terminé, il est possible de consulter le tracé GPS de l'appel.
    * Explication : Permet de consulter le cheminement d'un appel réparti automatiquement (répartition dans les zones, reprises et refus, no loads, etc.). Voir [Explication](informations-dappel.md#explication) ci-dessous.
17. Restriction d'appel : Les restrictions cochées durant la prise de l'appel.

## Explication

Le cheminement complet d'un appel peut être consulté grâce au boutton `Explication`.

{% tabs %}
{% tab title="1re action" %}
<div align="center"><figure><img src="../../.gitbook/assets/image (24).png" alt=""><figcaption></figcaption></figure></div>

Toutes les informations visibles permettent d'avoir un détail précis de l'ordre de répartition de l'appel.

Dans l'exemple ci-dessus, l'appel a été attribué au #413. Nous pouvons constater qu'il était premier dans la zone, inscrit depuis 14h39. Le suivant en liste était le #300, inscrit depuis 14h42, et ainsi de suite.

Nous voyons le type de véhicule, leur distance par rapport à l'adresse demandé par le client.
{% endtab %}

{% tab title="2e action" %}
<figure><img src="../../.gitbook/assets/image (25).png" alt=""><figcaption></figcaption></figure>

Le véhicule a fait NoLoad en arrivant à l'adresse.
{% endtab %}

{% tab title="Untitled" %}
<figure><img src="../../.gitbook/assets/image (26).png" alt=""><figcaption></figcaption></figure>

Dans cet exemple, le système a repris l'appel. Le chauffeur a "refusé" l'appel. Le système a aussi appliqué une pénalité de type `Perte Position`.
{% endtab %}
{% endtabs %}
