# Benin Land Parcels & NUP Lookup MCP (Bénin)

[Français](#français)

Connect your AI assistant (Claude, ChatGPT, Cursor) to [BumiAtlas](https://bumiatlas.com) for Beninese land research through the Model Context Protocol (MCP).

This listing is a focused entry point for:

- ~631k surveyed parcels from the ANDF (Agence Nationale du Domaine et du Foncier) national cadastre, mostly in the southern départements
- Parcel lookup by NUP (numéro unique parcellaire) or titre foncier number, narrowed by commune, or by coordinates
- Register status, recorded right (ownership or presumed ownership), digital-cadastre or titled, the survey's open issue (unknown owner, disputed, …) and surveyed area
- The declared zones at a point: classified forests, state domain (ZDUP), titles in progress, rivers — the only outlines in the unsurveyed north
- Satellite and street map images of a parcel and its neighbours, labelled by NUP

Parcels have no holder names. The ANDF reserves all rights to this data: use it for your own information and credit the source.

## Connect

```
https://bumiatlas.com/mcp/benin
```

Add it as a custom connector in any MCP client and sign in with Google. Tools, examples and data notes: [bumiatlas.com/mcp-docs/benin](https://bumiatlas.com/mcp-docs/benin).

- **Claude:** Settings → Connectors → Add custom connector, paste the URL, then Connect.
- **ChatGPT:** Settings → Apps & Connectors → Advanced → Developer mode, then Create with the URL and OAuth authentication.

## Tools

| Tool | Description |
|---|---|
| `BJ_parcel_search` | Find parcels by NUP or titre foncier (narrowed by commune), or by `latitude, longitude` with the declared zones there; each result is the whole record, the boundary as GeoJSON on request |
| `BJ_parcel_image` | Satellite or street map image of a parcel or point, with every parcel in view outlined and labelled with its NUP |

## Example prompts

- *"Which parcel is at 6.3654, 2.4183? Is it titled?"*
- *"Find the parcel with titre foncier 1234 in Cotonou."*
- *"Is this point in a classified forest or state domain?"*
- *"Does the survey record an open issue on this parcel?"*

## Data source

Parcels © Agence Nationale du Domaine et du Foncier (ANDF), Bénin (cadastre.andf.bj). All rights reserved by the ANDF; not a legal land record.

## Français

Connectez votre assistant IA (Claude, ChatGPT ou Cursor) à [BumiAtlas](https://bumiatlas.com) via le Model Context Protocol (MCP) pour vos recherches foncières au Bénin.

- ~631 000 parcelles levées du cadastre national de l'ANDF, surtout dans le sud
- Recherche par NUP, titre foncier ou coordonnées, avec les zones déclarées (forêts classées, domaine de l'État)
- Images satellite et plan d'une parcelle et de ses voisines

Aucun nom de titulaire. L'ANDF se réserve tous les droits sur ces données.

**Connexion :** ajoutez `https://bumiatlas.com/mcp/benin` comme connecteur personnalisé dans votre client MCP et connectez-vous avec Google. Les noms des outils sont en anglais, mais l'assistant peut répondre en français.
