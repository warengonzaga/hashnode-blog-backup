---
title: "How to Enable Buy Me a Coffee to your Open Source Project on GitHub?"
seoTitle: "Enable Buy Me a Coffee on GitHub Projects"
seoDescription: "Learn to add a Buy Me a Coffee button to your GitHub project in simple steps, supporting open-source funding"
datePublished: Tue Mar 19 2024 07:25:46 GMT+0000 (Coordinated Universal Time)
cuid: clty1vs1l000209jo3slh2jj3
slug: how-to-enable-buy-me-a-coffee-to-your-open-source-project-on-github
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1710833066546/0465aef4-b320-4c89-b2d8-5848087ac04f.jpeg
tags: tutorial, github, opensource

---

Just recently, Buy Me a Coffee [announced](https://twitter.com/buymeacoffee/status/1769746574215930295) support for GitHub sponsors. This is really BIG news for open-source maintainers like me, as [we have been fighting for it for years](https://building.buymeacoffee.com/feature-requests/p/github-sponsorship).

This means that Buy Me a Coffee now supports its own syntax for the `FUNDING.yml` file, which is `buy_me_a_coffee` followed by your username. It displays like this.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1710831661462/ae8f8209-100d-494f-9f59-b249e232b974.png align="center")

Beautiful right? This is like a dream come true for me as compare before it displays like this as we use `custom` syntax just to support Buy Me a Coffee platform.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1710831846589/5d720d21-0b65-479a-916c-d5b7fda42b61.png align="center")

This is a significant improvement after years of waiting! If you're curious about which platforms are supported, you can learn more about the GitHub sponsors button [here](https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/customizing-your-repository/displaying-a-sponsor-button-in-your-repository).

Alright, now that we understand what this is all about, I'll show you how to enable this feature on your open-source project. This way, your users can support your project by actually buying you a coffee. ☕

Without further ado, let's get started! 🚀

## Steps

1. Clone your GitHub project repository.
    
    ![Clone GitHub repository using GitHub CLI](https://cdn.hashnode.com/res/hashnode/image/upload/v1710825225915/33501287-21a1-46ab-b8ef-3680fad106fa.png align="center")
    
    In my case, I prefer to use GitHub CLI as it is convenient for me to clone projects easily in my local machine. You can use whatever you prefer to clone your project.
    
    ![Example of cloning GitHub repository locally using GitHub CLI.](https://cdn.hashnode.com/res/hashnode/image/upload/v1710825439611/502bf100-4f93-42d3-a2c6-a2a39c85b4c8.png align="center")
    
    Here's how I clone my project, as you can see cloned directly to my local machine. I'm using WSL on Windows 11. 😅
    
2. If you haven't already, Create a `.github` folder at the root of your project.
    
    ![Example of navigating to project folder and showing the .github folder.](https://cdn.hashnode.com/res/hashnode/image/upload/v1710825568876/4fecaac9-5367-457f-bdac-196c38bee796.png align="center")
    
    After cloning the project, you'll need to navigate to the project folder. In my case, I use the terminal and `cd` command to do this. I have already a `.github` folder due to the fact that I'm using Buy Me a Coffee URL before using `custom` syntax to add my Buy Me a Coffee profile.
    
3. Inside your `.github` folder, you have to create another file called `funding.yml`.
    
    ![](https://cdn.hashnode.com/res/hashnode/image/upload/v1710826185948/25a6a956-5629-41dc-ac18-1093be50e1e2.png align="center")
    
    Navigate inside the `.github` folder and create a file name `funding.yml`. In my example, I have already a file name so I will not create another one.  
      
    You might be wondering why I don't name it as `FUNDING.yml`? This is because it is my preference if the file is not so important inside my project I don't use uppercase. Both lowercase and uppercase works when setting up your funding file for GitHub.
    
4. Open `funding.yml` file in your favorite code editor in my case I'll use VS Code.
    
    ![](https://cdn.hashnode.com/res/hashnode/image/upload/v1710829717353/3e2ca87b-c0c7-4e5b-b62b-58631ddf7919.png align="center")
    
    It will open a VS code in my local machine so I can modify the file and enable Buy Me a Coffee button to my opensource project.
    
5. Use the following syntax below to specify Buy Me a Coffee platform as your GitHub sponsors button.
    
    ![](https://cdn.hashnode.com/res/hashnode/image/upload/v1710829652573/8639b708-7ffb-4166-be1a-42561d3dab8b.png align="center")
    
    You can use comment syntax for your YAML file like in my example. If your account has GitHub sponsors enabled you can add it to your funding tile too. In my case, I have both. You can [apply here](https://github.com/sponsors) if you want!
    
6. Commit your changes, and push it!
    
    ![](https://cdn.hashnode.com/res/hashnode/image/upload/v1710830143528/4f053810-c5d1-45aa-974e-127229e3da88.png align="center")
    
    Once, you update your `funding.yml` file you need to commit your changes and push your updates. In my case, I'm using an AI-powered commit message tool called "[Magic Commit](https://github.com/warengonzaga/magic-commit)" or "[magicc](https://npmjs.com/package/magicc)" in short. If you like doing manual then follow the Git flow below.
    
    ![](https://cdn.hashnode.com/res/hashnode/image/upload/v1710830443184/f1c6c923-4fa6-42b6-81f5-9ea5a299dbed.png align="center")
    
7. That's it, you should be able to see the **Buy Me a Coffee** button from your GitHub project's repository homepage.
    
    ![](https://cdn.hashnode.com/res/hashnode/image/upload/v1710830645059/fc39a6f3-977e-4573-b1f7-7951e0848c58.png align="center")
    

Enjoy your coffee and happy building! ☕

See you in my next blog... 💖

%%[sponsor]