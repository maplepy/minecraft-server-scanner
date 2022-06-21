# What's it do?
Uses [masscan](https://github.com/robertdavidgraham/masscan/) to scan the internet for Minecraft® servers,
then uses Dinnerbone's [mcstatus](https://dinnerbone.com/minecraft/tools/status/) to grab the GameSpy3 data,
cleaning up the process of doing it manually.

Tested with:
- Ubuntu - 21.10 - [Impish Indri](https://cdimage.ubuntu.com/daily-canary/current/)
- Kali Linux - [Bleeding Edge](https://cdimage.kali.org/kali-images/kali-weekly/)
- masscan - [robertdavidgraham/masscan@`144c527`](https://github.com/robertdavidgraham/masscan/commit/144c527ed55275ee9fbb80bb14fbb5e3fcff3b7e)
- mcstatus - [Dinnerbone/mcstatus@`10cea64`](https://github.com/Dinnerbone/mcstatus/commit/10cea643fa3866063c6b5b327fe890213ecee7f2)
- mcc - [ORelio/Minecraft-Console-Client@`41b0325`](https://github.com/ORelio/Minecraft-Console-Client/commit/41b0325f45b3084ae66ced37e9311927360d6aa8)

# But why?
Purely because its easier to shorten the process by making it scripted, then I just cleaned it up for
public release, so other people can have fun joining random servers.

The process usually goes like this:
1. Scan ISP range.
2. See players online in a server.
3. Switch to the appropriate Minecraft® version.
4. Join the server.

Various reactions ensue, from "Hello?" to...

### Connection Lost
#### You are banned from this server.

# Screenshots
##### Starting a scan of 1 million AT&T routers (took 3 minutes)
![csh01](https://user-images.githubusercontent.com/6983255/111035107-f368d400-846c-11eb-8c88-670e83d16077.png)

##### Using `mcstatus` to display information about the servers
![csh02](https://user-images.githubusercontent.com/6983255/111035136-1bf0ce00-846d-11eb-8d37-93c90eede5bf.png)

##### Using `mcc` to log in to Minecraft® and join the servers
![csh03](https://user-images.githubusercontent.com/6983255/111035182-55293e00-846d-11eb-86d9-efbfbaed53ae.png)

##### Running the default creeper.sh script with MCC on a server
![csh04](https://user-images.githubusercontent.com/6983255/111035263-ae916d00-846d-11eb-95e4-d19cedbcce7c.png)

##### Completed scan after `mcstatus` and `mcc` have finished.
![csh05](https://user-images.githubusercontent.com/6983255/111035361-48f1b080-846e-11eb-9268-2043acfdc7a2.png)
