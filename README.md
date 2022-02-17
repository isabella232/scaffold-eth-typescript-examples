# 🏗 Scaffold-Eth Typescript

## Alchemy NFT API Example

This is an example of how to use the Alchemy NFT API to display NFTs in a wallet. Before running this example, head over to [Alchemy](https://alchemy.io) to create an account and an app. You'll need the app's API key to run this example.

After you've created the Alchemy app, grab the app key, and update `MainPage.tsx`:
![image](https://user-images.githubusercontent.com/23554636/154405743-6bb9a8a1-0199-42de-9360-fffa6542b8ac.png)

## Quick Start

Running the app

1. install your dependencies

   ```bash
   yarn install
   ```

2. start a hardhat node

   ```bash
   yarn chain
   ```

3. run the app, `open a new command prompt`

   ```bash
   # build hardhat & external contracts types
   yarn contracts:build
   # deploy your hardhat contracts
   yarn deploy
   # start vite
   yarn start
   ```


## NFTs
Enter in any address/ens in the input field to see the owners NFTs. It will parse the metadata of the NFT for the image, title, and description fields. For ENS names, it will use the ens metadata service to get the metadata.
![image](https://user-images.githubusercontent.com/23554636/154405848-61b23fab-13fc-40d1-9fd3-e1345b78be80.png)

A limitiation with this example is that you can only see a maximum of 100 NFTs. The Alchemy API does support paging though, if you need it.

