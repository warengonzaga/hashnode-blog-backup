---
title: "How to Recover the Ownership of Your thirdweb Pre-built Contract?"
seoTitle: "Recover Ownership of Your thirdweb Contract"
seoDescription: "Learn to recover and secure your thirdweb contract ownership without gas fees using our gasless method guide. Perfect for compromised admin wallets"
datePublished: Mon Mar 18 2024 13:54:36 GMT+0000 (Coordinated Universal Time)
cuid: cltx0byw300010ajt30rmaov6
slug: how-to-recover-the-ownership-of-your-thirdweb-pre-built-contract
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1710769776549/07edfd35-0d54-4b8c-af40-aa63f071f06e.jpeg
tags: tutorial, javascript, web3, thirdweb

---

This is useful if the admin of your contract is compromised. For example, if you add a balance to your admin wallet address and it unexpectedly gets transferred to a random address, changing it becomes challenging without gas to assign a new one.

In this guide, you'll learn how to change your admin wallet to a new one without needing to spend gas from your compromised wallet address, using the thirdweb gasless method. Without further ado let's get started! 😎

## Setup

1. Do `npx thirdweb create app --node --javascript --evm`
    
2. Rename the `.env.example` to `.env`
    
3. Copy and paste this to your `.env`
    

```plaintext
WALLET_PRIVATE_KEY=
THIRDWEB_SECRET_KEY=
RELAYER_URL=
```

4. After that, fill out the information needed.
    
5. Get the private key of the compromised wallet and paste it as a value to `WALLET_PRIVATE_KEY=`
    
6. Get the `secret key` from this https://thirdweb.com/create-api-key
    
7. Get the `relayer_url` from this tutorial https://blog.thirdweb.com/guides/setup-gasless-transactions
    
8. Copy and paste the code below to your local `index.js`
    

```javascript
import { config } from "dotenv";
import { ThirdwebSDK } from "@thirdweb-dev/sdk";

config();

const newAdmin = "0x...";
const contractAddress = "0x...";

const main = async () => {
  if (!process.env.WALLET_PRIVATE_KEY) {
    throw new Error("No private key found!");
  }

  try {
    const sdk = ThirdwebSDK.fromPrivateKey(process.env.WALLET_PRIVATE_KEY, 'polygon', {
      gasless: {
        openzeppelin: {
          relayerUrl: process.env.RELAYER_URL, // Learn more: https://blog.thirdweb.com/guides/setup-gasless-transactions/
        },
      },
      secretKey: process.env.THIRDWEB_SECRET_KEY,
    });

    const contract = await sdk.getContract(contractAddress);
    // run this first so you can set it as owner.
    const tx = await contract.roles.grant("admin", newAdmin);
    // Uncomment this, and comment the code above ^ after you set the newAdmin as admin.
    // const tx = await contract.owner.set(newAdmin);

    console.log(tx);

  } catch(error) {
    console.error("Something went wrong: ", error);
  }
};

main();
```

4. Fill in the information for the variables.
    

```plaintext
const newAdmin = "0x...";
const contractAddress = "0x...";
```

9. Run the code by doing `node index.js`
    

## Usage

1. After the setup, run the script straight. `node index.js`
    
2. Comment on this part by adding `//` in front of it.
    

```plaintext
const tx = await contract.roles.grant("admin", newAdmin);
```

3. Then, uncomment this part. By removing the `//` in front of it.
    

```plaintext
const tx = await contract.owner.set(newAdmin);
```

4. Run again the script. `node index.js`
    

---

That's it! ✨ See you on my next blog... 💖

%%[sponsor]