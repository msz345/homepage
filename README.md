# Homepage

Personal setup of my homepage, which caused my some headaches due to lacking real world examples. That's why I make it public.

My homelab consits of a Proxmox cluster, and some docker VMs. In order to not have too many widget visable at the same time (loading time or cluttering), I spilt them up into tabs.
Further I added my family calendar, and some useful bookmarks to the homepage.

<img width="1588" height="1978" alt="image" src="https://github.com/user-attachments/assets/0495f88d-8c91-446e-ae1e-78c4255d84b1" />

## Getting Started

I mainly use Proxmox to host my containers. Instead of setuping up each container itself, which I did many years, nowadays, I use the [Proxmox VE Helper-Scripts](https://community-scripts.github.io/ProxmoxVE/) community project. The project provides 400+ scripts to deploy and setup as much application - one is [gethomepage/homepage](https://github.com/gethomepage/homepage) itself.

After the homepage container is setup, I use Ansible to configure the homepage service, but you also can copy the files manually to its destination.
Just copy config files [/opt/homepage/config/](/opt/homepage/config/). Same for any picture that need to be copied to [/opt/homepage/public/images/](/opt/homepage/public/images/).
Finally, enter your secrets as environment viarables in [/opt/homepage/.env](/opt/homepage/.env).
