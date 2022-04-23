## Maintenance Your Windows Machine Like a Pro

Probably you are here because you have a Windows machine and it is getting slower and slower. Doing maintenance and optimization on your own requires time, research, and knowledge to do it right so you can avoid having additional Windows issues. I know the pain of having a Windows machine and doing maintenance, promise! 😅

![pain](https://media.giphy.com/media/4VUiK7uleZ7BcP21Sx/giphy.gif)

Let me share one story with you, one time I tried to do basic cleaning to my Windows machine using **Disk Cleanup** and I checked all the items there and delete them so I can free up some space. Do you know what happened? --- **Blue Screen of Death** shows! 🤦‍♂️

![microsoft](https://c.tenor.com/-aZGk99QVM8AAAAC/space-force-microsoft.gif)

With this wonderful experience using Windows, I motivated myself to learn about how can I effectively do maintenance and optimization without breaking my computer. I know that's a funny reason but that's my inspiration, that's why I created a tool that automates the optimization and maintenance of a Windows computer. 🤘

## 🧹 Cleaning Tool

![wrn-cleaner](https://cdn.hashnode.com/res/hashnode/image/upload/v1650394860088/103cEax2i.png)

Introducing, the WRN Cleaner! 🎉🎉🎉

It is a maintenance tool that can automatically or manually clean up your Windows machine in a simple and reliable way. It is designed specifically for Windows machines only. The motivation behind this project is to clean up Windows machines in an automated way with pre-configured optimization techniques. 😉💻🧹

### ⚡ Features

I'm using the native approach in cleaning Windows machine compare to other tools out there. Check out the different native Windows utility to automate the maintenance and optimization. 🔥

Here's the cleaning process in sequence. 🧹

- Disk Cleanup
- Defragment (HDD)
- Retrim (SSD)
- Checks System File
- Cleans Recycle Bin
- Cleans Temp Folder
- Cleans Prefetch Folder
- Clears Windows Error Log
- Auto or Manual Shutdown and Reboot When Done

***Disk Cleanup*** - As you may notice that I place the **Disk Cleanup** in the top of the cleaning process, why? My reason is that, this is the only native maintenance utility in Windows that needs user interaction. It is good to get the attention of the user to finish all the steps before leaving the program running. Placing the **Disk Cleanup** somewhere in the process will prevent the whole process to finish if the user is not attended causing the program to hang and not able to complete the cleaning process. Make sense? 😅

***Defrag / Retrim*** - Last year, I bought SSD to upgrade my workstation, but here's the question can I defrag my SSD? The answer is no! It has been a requested feature to the tool to support SSD enabled Windows machine. I started to research about this feature request and I found out that the Windows' **Defrag** utility software has optimization feature to work with SSDs which is the **Retrim**! The tool can safely detect and apply the necessary optimization for your storage device. 🤘

***System File Checker*** - Built-in utility for Windows machine for checking and restoring corrupted system files. That's it! 😅

***Recycle Bin / Temp Folder / Prefetch Folder*** - The tool cleans your recycle bin, temp folder and files, and prefetch folder to free up some storage. 👊

***Windows Error Log*** - This can be helpful to reduce the noise in your Windows logs by deleting old error logs. 🤝

> ⚠ **Reminder**: It is recommended to use this tool once every month.

## 🧰 Maintenance

![maintenance](https://c.tenor.com/xuwfj5uz2B8AAAAC/gopi-bahu.gif)

Now we have the tool, we don't have to worry about doing the same mistake I made in the past. 🤣 It is so simple to use my cleaning tool, just follow the usage below... 👀

1. Get the [latest stable version](https://github.com/warengonzaga/wrn-cleaner/releases).
2. Run the batch script file as an **Administrator**.
3. Follow the on-screen instructions.
4. Wait...
5. Done!

> ⚠ **Reminder**: When you start to run the program the first cleaning method would be **DiskClean** so be careful on this one, don't check or uncheck things here. It is set to the default configuration and all you have to do is to click ok or next.

## 🔐 Security

![security](https://c.tenor.com/YbmQHDSJvbkAAAAC/thumbs-up-hacker.gif)

Some of you may know that I'm a cybersecurity researcher by trade and security is very important to me. The maintenance tool I made is safe to use as I'm also using it, I mean you can read the entire source code in the official GitHub repository. 😅

In addition, you can check the [VirusTotal result here](https://www.virustotal.com/gui/url/092c4998fbb4b0bb8ff569d81dd92dffdf61edd3d6c37e591f5411b0bd948ab0/detection). 😉

If in any case, you are able to find a potential security bug then feel free to reach out to me or report it directly to my bug bounty partner which is the [huntr.dev](https://huntr.dev) go and get some CVEs. 👀

They pay security researchers for finding vulnerabilities in any GitHub repository and maintainers for fixing them. Cool right? 👏

## 🐱‍👤 Last Words

![last words](https://c.tenor.com/R4_XacJ__O8AAAAC/break-break-the-ice.gif)

Having a Windows machine can be painful as hell but this is where I started and this is all I have. I'm planning to get a new machine with Windows OS installed soon. Yeah I'm very comfortable with Windows machine as my main personal computer. For work purposes I would probably use Apple machine as it is very reliable in that use case, but that's really really soon. 🤞

Cleaning your machine can be painful too if you don't know the basics, that's where the tools become useful. For me, don't rely too much using tools still you have to learn the basics. 👊

The tool I made uses the native cleaning process for Windows. I just automate these steps and applied my years of experience in maintaining and optimizing Windows machine as I work before as technical support. ⚡

So yeah, I hope you learned a lot and hope this blog helps!

**Docs**: *[docs.warengonzaga.com/wrn-cleaner](https://docs.warengonzaga.com/wrn-cleaner)*

**Repo**: *[github.com/warengonzaga/wrn-cleaner](https://github.com/warengonzaga/wrn-cleaner)*

---

📢 Nominate me ([@warengonzaga](https://warengonzaga.com)) as a **[GitHub Star](https://stars.github.com/nominate)**. If you appreciate my hard work, passion, and dedication to open source projects like this.

Cheers! 🚀👌 See you on my next blog...