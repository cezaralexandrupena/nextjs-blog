---
title: 'MongoDB public IP binding in next.js'
date: '2022-03-30'
---
I spent more than three days last week trying to figure out how to connect to local MongoDB through the public IP adress.
This is what I learned:

- Enable your **firewall**.
- _Don't worry about it_.

Next.js -as long as we're talking about Server Side Rendering-, won't need to run mongodb through the public ip as long as they both run inside the same machine. Therefore external users don't need that type of access.
The server itself will handle everything and deliver to the user afterwards. When time comes we'll talk about Next.js running in a dedicated server and database running in a cloud network.

Till then, don't waste development time the same way I did.
