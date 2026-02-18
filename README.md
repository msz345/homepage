# Homepage

Personal setup of my homepage, which caused me some headaches due to lacking real world examples. That's why I make it public.

My homelab consits of a Proxmox cluster, and some docker VMs. In order to not have too many widget visable at the same time (loading time or cluttering), I spilt them up into tabs.
Further I added my family calendar, and some useful bookmarks to the homepage.

<img width="1569" height="829" alt="image" src="https://github.com/user-attachments/assets/0c1fc2f3-3265-49a0-8f34-b83171910983" />


<img width="1566" height="1197" alt="image" src="https://github.com/user-attachments/assets/6a6c744f-4177-4055-b080-ca52988ea79f" />


<img width="1567" height="1957" alt="image" src="https://github.com/user-attachments/assets/ab84d733-0f96-4d46-9eb0-400dbdf47eb0" />

## Getting Started

I mainly use Proxmox to host my containers. Instead of setting up each container itself, which I did many years, nowadays, I use the [Proxmox VE Helper-Scripts](https://community-scripts.github.io/ProxmoxVE/) community project. The project provides 400+ scripts to deploy and setup as much application - one is [gethomepage/homepage](https://github.com/gethomepage/homepage) itself.

After the homepage container is setup, I use Ansible to configure the homepage service, but you also can copy the files manually to its destination.
Just copy config files to [/opt/homepage/config/](/opt/homepage/config/). Same for any picture that need to be copied to [/opt/homepage/public/images/](/opt/homepage/public/images/).
Finally, enter your secrets as environment viarables (HOMEPAGE_VAR_*) in [/opt/homepage/.env](/opt/homepage/.env).
