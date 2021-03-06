---



copyright:
  years: 2017
lastupdated: "2017-10-24"


---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:screen: .screen}
{:new_window: target="_blank"}
{:pre: .pre}
{:table: .aria-labeledby="caption"}


# Nouvelle configuration d'un serveur virtuel existant
{: #reconfiguring-virtual-servers}

Une fois qu'un serveur virtuel est mis à disposition, vous pouvez mettre à niveau ou rétromigrer sa configuration à tout moment.  

**Remarque importante :** Il existe plusieurs serveurs virtuels publics disponibles dans des versions prédéfinies. Pendant une durée limitée, vous pouvez modifier tout serveur virtuel disponible avant les versions prédéfinies. Il vous est ensuite demandé de migrer ou d'annuler les instances existantes et de faire une nouvelle commande. 

Vous ne pouvez pas modifier le nombre de coeurs individuels, la mémoire RAM ou la taille de disque d'un serveur virtuel utilisant des versions. Vous devez choisir une autre version pour laquelle les coeurs, la mémoire RAM et la taille dont vous avez besoin sont prédéfinis. La version de serveur virtuel sélectionnée détermine le nombre de coeurs, la mémoire RAM et les tailles de disque valides.  

Les serveurs virtuels dédiés sont personnalisables plus facilement. Vous pouvez donc modifier le nombre de coeurs individuels, la mémoire RAM et les tailles de disque.

Utilisez la procédure suivante pour reconfigurer un serveur virtuel existant.
{:shortdesc}

## Modification d'un serveur virtuel existant (utilisant des versions prédéfinies)
1. Accédez au portail [{{site.data.keyword.slportal_full}} ![External link icon](../icons/launch-glyph.svg "External link icon")](https://control.softlayer.com/) en utilisant vos données d'identification uniques. 
2. Dans la liste de terminaux, cliquez sur le nom du serveur virtuel à reconfigurer.
3. Sur l'onglet **Configuration**, vous pouvez cliquer sur **Modifier** ou **Modifier la configuration de l'unité** pour mettre à jour les éléments suivants. 
  <dl>
  <dt>Taille</dt>
  <dd>Sélectionnez une nouvelle taille.</dd>
  <p><note>Remarque : Lorsque vous modifiez une version qui utilise le stockage local, vous ne pouvez pas utiliser de version n'en utilisant pas. De la même façon, lorsque vous modifiez une version qui utilise un stockage non local, vous ne pouvez pas utiliser de version en utilisant.
  </note></p>
  </dl>
4. Une fois que vous avez défini des modifications pour le serveur virtuel, finalisez la mise à jour de la configuration.
  <dl>
  
  <dt>Date de mise à niveau</dt>
  <dd>Vous pouvez cliquer sur la case à cocher Immédiatement pour une mise à jour immédiate ou planifier l'heure de la mise à jour.</dd>

  <dt>Heure de la mise à jour</dt>
  <dd>Entrez la date (AAAA-MM-JJ) d'application de la mise à jour.</dd>

  <dt>Remarques</dt>
  <dd>Entrez des remarques relatives à votre terminal. </dd>
  </dl>

5. Cliquez sur **Continuer**.
6. Vérifiez la confirmation de votre commande.  Cliquez sur **Editer** pour modifier votre mise à niveau.
7. Cliquez sur **Confirmer** pour confirmer votre commande et appliquer les modifications à votre terminal.

## Modification d'un serveur virtuel existant (avant les versions prédéfinies) ou d'un serveur virtuel dédié
1. Dans la liste de terminaux, cliquez sur le nom du serveur virtuel à reconfigurer.
2. Sur l'onglet **Configuration**, vous pouvez cliquer sur le lien de **mise à niveau de coeur ou de mémoire RAM** pour mettre à jour les éléments suivants.  
  
|   Options de mise à niveau |  Description                                                                                                |
| ----------------------- | ----------------------------------------------------------------------------------------------------------- |
| Date de mise à niveau      | Entrez la date (AAAA-MM-JJ) d'application de la mise à jour.                                                |
| Heure de mise à niveau     | Sélectionnez l'heure dans les zones déroulantes afin d'indiquer l'heure à laquelle la mise à jour doit être active, ou cochez la case **Immédiatement** pour une mise à jour immédiate.  |
| Coeurs                     | Sélectionnez le nombre de coeurs pour la mise à jour. |
| RAM                        | Sélectionnez la quantité de mémoire RAM à appliquer à votre terminal pour la mise à jour, si applicable.   |
| Vitesses de port Uplink    | Sélectionnez les vitesses du nouveau port de liaison montante. |
| Bande passante publique    | Sélectionnez la quantité (en Go) de bande passante publique pour votre terminal.   |
| Premier disque – Cinquième disque | Sélectionnez l'option d'espace disque/stockage pour le premier disque, le cas échéant. Pour plus d'informations, voir **Remarques relatives aux disques** ci-dessous.
|
| Remarques                   | Entrez des remarques relatives à votre terminal.                                                                 |
{: caption="Tableau 1. Options de déploiement" caption-side="top"}   
  
  **Remarques relatives aux disques :**
  * Un stockage de type local ou SAN est disponible. Vérifiez votre sélection pour vous assurer que l'option de stockage choisie est correcte. 
  * Pour les serveurs virtuels publics, si vous effectuez la mise à niveau du stockage local et que vous avez besoin de coeurs ou de mémoire RAM supplémentaires, vous risquez de perdre votre disque secondaire. Lorsque vous modifiez une version de serveur virtuel qui utilise le stockage local, la version est prédéfinie pour vous et les versions qui ne sont pas comparables ne peuvent pas être sélectionnées.
3. Cliquez sur **Continuer**.
4. Vérifiez la confirmation de votre commande.  Cliquez sur **Editer** pour modifier votre mise à niveau.
5. Cliquez sur **Confirmer** pour confirmer votre commande et appliquer les modifications à votre terminal.
