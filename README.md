<div align="center">
    <figure>
        <div>
            <img src="/images/icon_ha.png" alt="" width="128" height="128" />
        </div>
    </figure>
</div>
<h2 align="center">
   Installation, configuration et matériel<br/>pour Home Assistant<br/><br/><sup>par Mathieu Longpré</sup>
</h2>

## Table des matières

1. **[Introduction](#introduction)**
2. **[Équipement](#équipement)**
3. **[Réseau domotique](#réseau-domotique)**
4. **[Dell Wyse 7020](https://github.com/domolys/public/blob/main/WYSE-7020.md)**: spécifications
5. **[Wiki](https://github.com/domolys/public/wiki)**: installations

<br/>

## Introduction
En tant qu'utilisateur de Home Assistant depuis 2019, j'ai vite réalisé que bien que s'agisse d'une simple intégration domiciliaire, le succès de mon installation et de cette aventure résidait tout d'abord dans une bonne documentation. Ce dépôt se veut ainsi un partage des différents chapitres du développement de mon intégration.
En 2020 l'équipe de développement a voulu éclaircir les différents types d'installation de Home Assistant. Avant d'aller plus loin, il est important de comprendre en quoi consiste les différentes variances d'installations:  

**Home Assistant:** Il s'agit de l'installation la plus complète qui consiste à dédier une machine physique, ou virtuelle, à l'ensemble de la solution sous la forme d'un système d'exploitation.  

**Home Assistant Container:** Se limite à l'installation du noyau principal sous forme de conteneur.  

**Home Assistant Core:** Se limite à l'installation du noyau principal directement sous Python.  

**Home Assistant Supervised:** Consiste à installer l'ensemble de la solution sur un système d'exploitation autre que celui développé à cette fin. À ce jour, seul Debian 11 est supporté, et ainsi fortement recommandé.  

<br/>

## Équipement
Lorsque vous adoptez Home Assistant, l'équipement sur lequel votre solution est installée deviendra aussi important que votre connexion internet. Tout comme un routeur, cet équipement sera appelé à fonctionner en tout temps. Pour cette raison, j'accorde une importance particulière à ces points:  

**Consommation énergétique:** La solution devra consommer entre 5 et 10 watts pour un coût annuel d'utilisation entre 3$ et 8$. Consommation du serveur exclusivement: 10W x 24H x 365J x 0.065$ ÷ 1000 = 5.70$  

**Coût de l'équipement:** Une solution domotique élargie peut coûter très cher étant donné l'étendu des dispositifs requis. Pour cette raison, le coût du matériel sur lequel Home Assistant est installé ne devrait pas dépasser 200$.  

**Solution de remplacement:** Prévoir une solution de rechange en cas de panne de matériel. Prévoir une méthodologie de sauvegarde automatique.  

**Toujours actif:** Le matériel assurant la connexion internet ainsi que Home Assistant devraient être alimentés de façon continue.  

<br/>

## Réseau domotique

<div align="center">
    <figure>
        <div>
            <img src="/images/diagram_ha_hardware.png" alt=""/>
        </div>
    </figure>
</div>
