# Docker_Recipes
A Collection of Docker-Compose Files i use.

Those docker-compose files are stripped of information which are security sensitive.

Furthermore do i not use Placeholder - IPs or something similar, cause it allways anoyed me to see a compose file where they used a port for something, you may not want to use yourself ( especially when you are beginner and you have no clue what you want to use ( for example Port 465 vs 587 with Mailserver )). I will just write Port and you put in the Port you want. This will lead to not being able to past and instantly deploy, but it will lead to a better result.

One thing you will notice in my compose files is that i often use https ( 80 ) instead of https ( 443 ), because i dont need network encryption behind my Reverse Proxy. If it's already encrypted or it isn't much work, i sure will use encryption, but i won't create certificates etc. Firewall and Reverse Proxy do that, so keep in mind, you will want a Reverse Proxy with a working certificate ( for example from Lets Encrypt ) for it.

I love the Idea of Containers having static IP's, so i configured my compose files to use static ips. If you dislike my ranges, change them to whatever you want.