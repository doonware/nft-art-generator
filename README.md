# Generative NFT Art Engine + Moralis

## Quick Launch 🚀

Via terminal, navigate to root directory:

```sh
npm install

```

Go to [Moralis.io](https://moralis.io/) to create your server instance. Then rename .env-example file to .env and add your Moralis server credentials.

_Note_: To find your xAPI key: https://deep-index.moralis.io/api-docs/#/storage/uploadFolder

Create your layered artwork and split into folders in `./input` and configure your collection to match your layer structure and preferences accordingly by editing `./input/config.js`:

Finally, via terminal in the project directory run:

```sh
node index.js

```

This injects the mutagen that will bring your Moralis mutants ALIVE!

## Minting ⛓

Copy Solidity contract to [⚙️ Remix IDE](https://remix.ethereum.org/) for test and deplyment, but first edit code to point to your meta data's IPFS folder 'metahash/CID'. You can get this, saved in dasboard of your Moralis server instance in row of 'metahash' column.

```sh
constructor()
    ERC1155(
        "ipfs://INSERT_YOUR_CID_METAHASH/metadata/{id}.json"
    )
{
```
