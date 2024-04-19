---
title: "How to Set Up thirdweb Engine Quickly On Your Local Machine"
seoTitle: "Quick Setup Guide for thirdweb Engine"
seoDescription: "Learn to set up thirdweb Engine locally for Web3 projects using Docker, Git, and NodeJS with this easy guide"
datePublished: Fri Apr 19 2024 17:34:26 GMT+0000 (Coordinated Universal Time)
cuid: clv6y9xxc000208l9g1tuduc9
slug: how-to-set-up-thirdweb-engine-quickly-on-your-local-machine
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1713547858233/0ce4cce2-3f6e-444a-9252-aec8ac2e904c.jpeg
tags: tutorial, docker, apis, localhost, blockchain, rest-api, web3, thirdweb

---

Previously, we learned [how to deploy the thirdweb Engine in less than 3 minutes on the Railway](https://blog.warengonzaga.com/how-to-deploy-a-self-hosted-thirdweb-engine-on-railway-in-less-than-3-minutes) platform using the template we created for the community.

In this blog, you'll learn how to deploy it on your local machine so you can explore and experiment with the [thirdweb Engine](https://thirdweb.com/engine) for your next or current Web3 project.

## Requirements

* [Docker](https://docs.docker.com/get-docker/)
    
* [Git](https://git-scm.com/downloads)
    
* [NodeJS](https://nodejs.org/en/download/)
    
* Any code or text editor. ([VS Code](https://code.visualstudio.com/), [Vim](https://vim.org), or [Nano](https://nano-editor.org))
    
* [**thirdweb API secret key**.](https://portal.thirdweb.com/account/api-keys#:~:text=Secret%20Key%2D%20Used%20to%20access%20the%20enabled%20thirdweb%20infrastructure%20services%20by%20identifying%20and%20authenticating%20your%20application%20from%20a%20backend.%20Sharing%20or%20exposing%20this%20key%20to%20others%20is%20unsafe%20because%20it%20grants%20access%20to%20all%20services.)
    
* [**Wallet addr**](https://portal.thirdweb.com/account/api-keys#:~:text=Secret%20Key%2D%20Used%20to%20access%20the%20enabled%20thirdweb%20infrastructure%20services%20by%20identifying%20and%20authenticating%20your%20application%20from%20a%20backend.%20Sharing%20or%20exposing%20this%20key%20to%20others%20is%20unsafe%20because%20it%20grants%20access%20to%20all%20services.)[**ess**.](https://portal.thirdweb.com/glossary/wallet) (any EVM-compatible wallet address)
    

<div data-node-type="callout">
<div data-node-type="callout-emoji">💡</div>
<div data-node-type="callout-text">Are you looking for a managed thirdweb Engine? <a target="_blank" rel="noopener noreferrer nofollow" href="https://thirdweb.com/dashboard/engine?requestCloudHosted" style="pointer-events: none">Try Cloud-Hosted</a>!</div>
</div>

## Steps

1. Open your terminal on your local machine and execute the command below. It will clone my scripts into a new folder called `engine`.
    
    ```bash
    git clone https://github.com/warengonzaga/thirdweb-engine-deploy-locally engine
    ```
    
    ![A screenshot of a command line interface where a user clones a GitHub repository named "thirdweb-engine-deploy-locally" into a local directory, lists files in a directory, and navigates between directories.](https://cdn.hashnode.com/res/hashnode/image/upload/v1713534926781/faf1e53f-6866-424e-9a40-1fa90c194f86.png align="center")
    
2. Navigate to the `engine` folder and open the file named `.env.example`. Fill out the required information. I prefer to use the Nano text editor in this guide because it is straightforward.
    
    ![A screenshot of a computer terminal showing the GNU nano text editor open with a file named ".env.example" containing environment variable settings for thirdweb engine.](https://cdn.hashnode.com/res/hashnode/image/upload/v1713536129747/7ee60a3a-39d6-4477-8741-039332f200ea.png align="center")
    
    | Variable | Description |
    | --- | --- |
    | `ADMIN_WALLET_ADDRESS` | The wallet address that will configure Engine from the thirdweb dashboard. |
    | `THIRDWEB_API_SECRET_KEY` | A thirdweb secret key was created on the [API Keys page](https://thirdweb.com/dashboard/settings/api-keys). |
    | `ENCRYPTION_PASSWORD` | Provide a string to encrypt sensitive data stored in DB. Do not change this value, or encrypted data will be inaccessible. |
    
    <div data-node-type="callout">
    <div data-node-type="callout-emoji">💡</div>
    <div data-node-type="callout-text">To save your changes in the Nano text editor, press <code>CTRL+X</code>. It will then ask you to confirm the save. Simply, press <code>Y</code> and then hit <code>ENTER</code> to complete the process.</div>
    </div>
    
3. After that, start Docker on your local machine and ensure it is running.
    
    ![Screenshot of Docker Desktop interface showing an empty state for running containers with informational tooltips about containers and how to run them.](https://cdn.hashnode.com/res/hashnode/image/upload/v1713540842021/05db84e4-f35f-4cb3-b0a4-51d513dad942.png align="center")
    
4. Now, return to your terminal and run `npm run start`, and it will handle everything for you. Watch your terminal pull the thirdweb engine docker image and set up your container. If you see the message below, your engine has been successfully deployed and is ready to use.
    
    ![A screenshot of a computer terminal displaying logs and warnings from a Node.js application, including messages about starting a PostgreSQL connection and listening on port 3005.](https://cdn.hashnode.com/res/hashnode/image/upload/v1713541903702/911d1a4f-b176-4518-b1e7-a5aa0f87701f.png align="center")
    
5. Lastly, visit your endpoint URL at `http://localhost:3005` , and you should see something like the example below. That's it! ✨
    
    ![A screenshot of a computer screen displaying a JSON response message that reads "Engine is set up successfully. Manage your Engine from https://thirdweb.com/dashboard/engine." in a code editor with a dark background.](https://cdn.hashnode.com/res/hashnode/image/upload/v1713543528514/5a751183-0030-4715-b3f0-662ae28efd5f.png align="center")
    

Now that you have the endpoint URL, let's import your instance to the thirdweb Engine dashboard. [Follow the steps here](https://blog.warengonzaga.com/how-to-deploy-a-self-hosted-thirdweb-engine-on-railway-in-less-than-3-minutes#heading-manage-ending-from-the-dashboard).

## Try Engine Examples

To explore and experience the capabilities of thirdweb Engine, try some of our [templates](https://thirdweb.com/templates). Here are some of the best templates we have today for building with thirdweb Engine.

### [Mintcaster](https://thirdweb.com/template/mintcaster)

![Screenshot of Mintcaster template](https://thirdweb.com/assets/templates/mintcaster.png align="left")

Bootstrap your own client on Farcaster, complete with a feed, cast functionality, and Sign-in with Farcaster auth, and add NFT minting functionality using the thirdweb Engine.

### [Phygital Experience](https://thirdweb.com/template/phygital-experience)

![Screenshot of Phygital Experience template](https://thirdweb.com/assets/templates/phygital-experience.png align="left")

Users can scan a QR code on a physical product to mint an NFT using the thirdweb engine. Perfect for buying and selling digital items physically.

### [Speed Racer](https://thirdweb.com/template/unreal_demo)

![Screenshot of Speed Racers template](https://thirdweb.com/assets/templates/speed-racer.png align="left")

Try this template with the thirdweb Engine and Unreal game engine to build your own racing game powered by the blockchain.

That's all! Enjoy, and keep building! 🫶