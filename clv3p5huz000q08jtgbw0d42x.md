---
title: "How to Deploy a Self-hosted thirdweb Engine On Railway In Less Than 3 Minutes"
seoTitle: "Deploy thirdweb Engine on Railway in 3 Minutes"
seoDescription: "Learn to deploy a self-hosted thirdweb Engine on Railway in under 3 minutes with this easy tutorial."
datePublished: Wed Apr 17 2024 10:55:43 GMT+0000 (Coordinated Universal Time)
cuid: clv3p5huz000q08jtgbw0d42x
slug: how-to-deploy-a-self-hosted-thirdweb-engine-on-railway-in-less-than-3-minutes
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1713548146982/4c6d458c-641e-45a0-9f5f-e18498e645e1.jpeg
tags: tutorial, apis, blockchain, rest-api, web3, railway, thirdweb, railway-app

---

Are you looking for a production-grade HTTP server to interact with any smart contract on any EVM? That's the thirdweb Engine!

[Engine](https://thirdweb.com/engine/) is a backend HTTP server that reads, writes, and deploys contracts on a large scale. It allows you to create and interact with backend developer wallets, supporting high throughput with automatic nonce and gas management. Think of this as your rail transport vehicle or train **Engine** for your **Railway**. 🚂

[Railway](https://railway.app/) is a deployment platform created to simplify the software development lifecycle. It starts with instant deployments and easy scaling and includes CI/CD integrations and built-in observability. Let's say this is the **Railway** track for your train **Engine**. 🛤️

In this tutorial blog, you'll learn how to deploy your self-hosted thirdweb Engine on the Railway platform in less than 3 minutes using our [community-contributed Railway template](https://railway.app/template/fcEVay). This is the official community Railway template maintained by the thirdweb community team.

Without further ado, let's deploy your **Engine** to its **Railway**. 🚂🛤️ (you get it?)

<div data-node-type="callout">
<div data-node-type="callout-emoji">ℹ</div>
<div data-node-type="callout-text">Are you looking for a managed thirdweb Engine? <a target="_blank" rel="noopener noreferrer nofollow" href="https://thirdweb.com/dashboard/engine?requestCloudHosted" style="pointer-events: none">Try Cloud-Hosted</a>!</div>
</div>

## Requirements

* [thirdweb API secret key](https://portal.thirdweb.com/account/api-keys#:~:text=Secret%20Key%2D%20Used%20to%20access%20the%20enabled%20thirdweb%20infrastructure%20services%20by%20identifying%20and%20authenticating%20your%20application%20from%20a%20backend.%20Sharing%20or%20exposing%20this%20key%20to%20others%20is%20unsafe%20because%20it%20grants%20access%20to%20all%20services.).
    
* [Wallet address](https://portal.thirdweb.com/glossary/wallet). (any EVM-compatible wallet address)
    

## Steps

1. Go to your Railway dashboard and create a "New Project."
    
    ![Railway platform showing options to create a new project, with a highlighted button for "New Project" on the top right. The Railway interface includes a sidebar with user information and a central area displaying project creation options such as deploying a GitHub repository or provisioning a database.](https://cdn.hashnode.com/res/hashnode/image/upload/v1713272787740/636b8689-6594-47b4-848b-33ea57c25764.png align="center")
    
2. On the new project page, search for "thirdweb" or "thirdweb Engine," and you will find the template we created.
    
    ![Railway deployment interface displaying a "New Project" screen with an option to deploy a web3 app using the "thirdweb Engine," described as an open-source server for scalable web3 apps. The background is dark with a subtle starry pattern.](https://cdn.hashnode.com/res/hashnode/image/upload/v1713272932738/d0ae83f5-de52-45ab-bb3d-a531210ddee0.png align="center")
    
3. You will be redirected to the deploy page. First, click the "Configure" button for the Postgres service. Lastly, save the configuration and return to this page.
    
    ![A screenshot of Railway deployment interface titled "Deploy Thirdweb Engine," featuring options to configure Postgres and Engine services, set against a dark background with a starry pattern.](https://cdn.hashnode.com/res/hashnode/image/upload/v1713341464873/2a451398-f164-445f-ad1f-160a86faee21.png align="center")
    
    ![Screenshot of Railway deployment interface titled "Deploy Thirdweb Engine," showing configuration options for a Postgres service including Docker image details, volume, and environment variables with a "Save Config" button at the bottom.](https://cdn.hashnode.com/res/hashnode/image/upload/v1713341688018/43f480be-f8e8-41aa-90cf-5e0b979e5912.png align="center")
    
4. Let's set up the thirdweb Engine service. Enter your wallet address into the `ADMIN_WALLET_ADDRESS` field, and then enter your "thirdweb API secret key" into the `THIRDWEB_API_SECRET_KEY` key input field. After that, save the configuration and return to the template deployment page.
    
    ![A screenshot of Railway interface for the thirdweb Engine, showing options to configure PostgreSQL and the Thirdweb Engine, with a dark background and a "Deploy" button at the bottom.](https://cdn.hashnode.com/res/hashnode/image/upload/v1713341935145/aa0322fa-0235-4734-a475-e294fd187a5f.png align="center")
    
    ![A screenshot of Railway configuration interface for deploying a Docker image, specifically "thirdweb/engine:latest". The interface displays fields for Docker image details, environment variables including 'ADMIN_WALLET_ADDRESS' and 'THIRDWEB_API_SECRET_KEY', and a 'Save Config' button.](https://cdn.hashnode.com/res/hashnode/image/upload/v1713342418431/b974c06a-3ce2-4d86-b9ff-1b66e445d125.png align="center")
    
5. All you have to do is click the "Deploy" button and wait.
    
    ![Screenshot of Railway deployment interface for "Thirdweb Engine" with options to configure and deploy services including "Postgres" and "Engine," both marked as "Ready to be deployed." The background is dark with a subtle star pattern.](https://cdn.hashnode.com/res/hashnode/image/upload/v1713342795793/b65e32eb-59eb-4fe4-8c9c-3539d4509d7c.png align="center")
    
6. In less than 3 minutes, your thirdweb Engine will be ready for use. Go to your Engine service &gt; Settings &gt; Networking &gt; Public Networking to find your endpoint URL.
    
    ![Screenshot of Railway web application interface showing settings for networking in a deployment environment, highlighting the public endpoint URL for an application named "engine-production".](https://cdn.hashnode.com/res/hashnode/image/upload/v1713343606568/2d1e63a8-6cb4-4855-80cc-625624219585.png align="center")
    
7. Open this endpoint URL in your browser, and you'll receive an API message response. This indicates a successful Engine installation. Be sure to save this; you will need it to import into your thirdweb Engine dashboard.
    
    ![A screenshot of a Railway interface showing a JSON response message stating "Engine is set up successfully. Manage your Engine from https://thirdweb.com/dashboard/engine." in a web browser.](https://cdn.hashnode.com/res/hashnode/image/upload/v1713343998368/5d6acc5f-ae45-44c9-883c-e6128b0e3594.png align="center")
    

### Manage Ending from the Dashboard

1. Now, let's import your endpoint URL to your thirdweb dashboard. Navigate to your [Engine dashboard](https://thirdweb.com/dashboard/engine) and select the "Import" button.
    
    ![A screenshot of a thirdweb user interface for a blockchain-related service called "Engine," featuring navigation tabs, account information, and sections for managing backend wallets and transactions. The interface includes options to import or create an instance of an Engine.](https://cdn.hashnode.com/res/hashnode/image/upload/v1713344362888/169c12c9-c95f-411c-bb5e-454c79b90223.png align="center")
    
2. Name your self-hosted thirdweb Engine, enter the endpoint URL from your Railway project, and click the import button. Follow the example provided below.
    
    ![A screenshot of thirdweb interface for importing an engine instance, featuring fields for name and URL, and buttons for "Cancel" and "Import".](https://cdn.hashnode.com/res/hashnode/image/upload/v1713344509842/2c6d53d1-e130-4abf-a59f-b30dfc347e41.png align="center")
    
3. After you import it, it should look like this. Go ahead and view and manage your self-hosted thirdweb Engine from your account dashboard.
    
    ![Screenshot of thirdweb web interface titled "Engine," describing it as an HTTP server for smart contracts, with options to manage instances and a link to an instance named "Engine on Railway."](https://cdn.hashnode.com/res/hashnode/image/upload/v1713344826533/fcdb8c51-1caa-4de0-a731-e0f6cb1b1f9a.png align="center")
    
4. Don't forget to create your **backend wallet** to execute write transactions and generate your **access token**. This will allow you to interact with your Engine API.
    
    ![Screenshot of thirdweb user interface for "Engine on Railway" showing sections for backend wallets and transactions with no data found, and tabs for Overview, Explorer, Relayers, Admins, Access Tokens, Webhooks, and Configuration.](https://cdn.hashnode.com/res/hashnode/image/upload/v1713345091101/fdf637fc-060d-4da6-9b16-f9a9cccf47a3.png align="center")
    
    ![Screenshot of thirdweb web interface for "Engine on Railway" showing a section for creating and managing API access tokens, with a button highlighted for creating a new access token.](https://cdn.hashnode.com/res/hashnode/image/upload/v1713345122537/8b9e406c-f512-4b60-8c84-0fe4c1f90ad6.png align="center")
    

## Testing

In this section, let's test your engine to see if it works. The simplest method is to make a direct request using curl in your terminal. Just replace the `<xxxx>` with your Railway endpoint URL and provide your access token from your thirdweb Engine dashboard.

We will send a GET request to read the contract information for `name` on the `base-sepolia-testnet` chain. Let's use `0xD1042CC90244beeE8E30e1655f1935C3e8BFB86a` as our test contract address.

```plaintext
curl -X 'GET' \
  'https://engine-production-<xxxx>.up.railway.app/contract/base-sepolia-testnet/0xD1042CC90244beeE8E30e1655f1935C3e8BFB86a/read?functionName=name' \
  -H 'accept: application/json' \
  -H 'Authorization: Bearer <your access token here>'
```

Copy and paste this command into your terminal and press enter. It should return a response with the name of our test contract. The name should be [Mata NFT](https://thirdweb.com/base-sepolia-testnet/0xD1042CC90244beeE8E30e1655f1935C3e8BFB86a).

![A screenshot of a terminal window displaying a command line interface where a curl command is executed to fetch data from an API, with the output showing JSON formatted response containing the result "Mata NFT".](https://cdn.hashnode.com/res/hashnode/image/upload/v1713346930114/c961ecdd-1bff-4ec3-8e92-eeded64b9279.png align="center")

You can also use the [Insomnia](https://insomnia.rest/) software to test your Engine. We performed a similar request using its graphical user interface (GUI). Enter your access token in the Bearer field as your authentication method, and then input your GET request URL. After that, click "Send." You should receive a 200 response code and the test contract's name.

![A screenshot of the Insomnia API client interface showing a GET request to a URL and the response displayed on the right side with the result "Mata NFT".](https://cdn.hashnode.com/res/hashnode/image/upload/v1713346646308/2ca884fa-1717-44c4-a993-0cbfb510469f.png align="center")

This is it. If you see a similar result, you're good to go! 🚂🛤️

## Update

You need to update the version manually from the Railway dashboard. To do this, navigate to your Engine service and redeploy the source.

![Screenshot of Railway deployment interface showing options for managing a Docker image deployment, including logs, restart, redeploy, and remove actions.](https://cdn.hashnode.com/res/hashnode/image/upload/v1713350921150/f5811d28-71c5-4c53-a7cc-efcad332d753.png align="center")

<div data-node-type="callout">
<div data-node-type="callout-emoji">ℹ</div>
<div data-node-type="callout-text">Are you looking for an effortless version update? <a target="_blank" rel="noopener noreferrer nofollow" href="https://thirdweb.com/dashboard/engine?requestCloudHosted" style="pointer-events: none">Try Cloud-Hosted</a>!</div>
</div>

Enjoy, and keep building! 🫶