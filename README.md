__In development!!__

<p align="center"><img src="https://github.com/user-attachments/assets/b9c357e0-e1c0-46c8-a8fd-a927a5cd40ac"></p><br>
<h1 align="center">Cloudflare Security</h1>

Hello there peeps! I've decided to create this repo as it concerns me about people's Cloudflare security as if newbies don't know how to protect their websites correctly, it could bring down whatever they're using their domain for (unless it's a big service like GitHub, Vercel, etc.) What this repo is about is to help them protect their websites. First, let's start with the basics.

# What is a DDoS Attack?

A Distributed Denial of Service (DDoS) is a cyper-crime attack that aims to disrupt / take down a network, service, or flood the service with tons of traffic which may end up slowing down their machine. The main goal of a DDoS attack is to take something down and make it harder for it to come back up. For more information I suggest reading this article written by Cloudflare: [cloudflare.com](https://www.cloudflare.com/learning/ddos/what-is-a-ddos-attack/)

# What are DDoS Attack Layers?

There are multiple layers of DDoS attacks. The smaller ones are a Layer 3 and Layer 4 DDoS attack. **Layer 3** DDoS attacks don't open many connections and provides reliable data delivery to the target. A **Layer 4** DDoS attack invovles TCP and UDP which most websites / game servers use. This can be a strong attack as if you don't set something up to block these fast attacks it may be fatal and shut down your machine completely. A **Layer 7** attack is one of the most fatal attacks. It acts like regular users and once it bypasses normal protection from your provider for example, it can fill the bandwidth very fast and eventually take down your machine. For more information I suggest reading this article written by Cloudflare: [cloudflare.com](https://www.cloudflare.com/learning/ddos/application-layer-ddos-attack/)

# How do I prevent this?

There isn't a bunch of ways if you want to install something internally. If you're hosting websites and such, there might be a way to prevent these attacks to happen using something called Cloudflare. Cloudflare is a domain management that provides a ton of security for their free plan, meaning you don't need to pay for much. Cloudflare offers security against DDoS attacks (if you set it up correctly), it offers more preformance to your website by caching big files, you can customize their SSL/TLS encryption, and much more. This documentation is focused around Cloudflare as it's one of the biggest anti-DDoS services that you can use if you set everything up correctly. Now, let's move onto the real steps.

# How do I setup Cloudflare so my DDoS attacks get blocked?

This honestly might be the biggest question yet. There are hundreds of people who search daily for anti-DDoS attacks because they're tired of getting hit by large amounts of attacks. Your search ends here however. First, let's cut it to the chase. If you're getting DDoSed via IP, there is nothing we can do. Cloudflare only works externally and blocks connections from, for example, **lezetho.co.uk**. If they get your IP from your domain this article is really useless unless you install something like Fail2Ban or setup IPTables to ban the IP. This article focuses around Cloudflare and external DDoS attacks that occur from your domain. Now, let's get to the real steps.

**How to block DDoS attacks from my domain using Cloudflare?**
Now, there's a series of ways to start off. Let's go from the basics.
