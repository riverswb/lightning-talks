# Botnets and the Internet of Things

## Botnets
### The fuck is a botnet?
* a botnet is a network of computers which have been infected with malware, allowing them to be remotely controlled.  
* botnets can consist of hundreds of thousands (even millions) of computers
* the infected computer becomes a part of the botnet when it is in contact with a remote server, or other bots, and takes commands from whoever is in control of the botnet
* the botnet's creator can decide what to do with the botnet later (download other types of malware or have the bots act together)

### What can you even do with a botnet?
* Many different purposes...
  * spam zomibes, DDoS zombie, click fraud zombie, anonymization proxy, CAPTCHA solving zombie
* a very common and profitable purpose is to have the bots act in unison to perform a DDOS attack on a web server
  * Hundreds, thousands, even hundreds of thousands (some resources report botnets controlling millions of machines) of computers would bombard a website with traffic at the same time, overloading it and causing it to perform poorly or be unreachable for people who actually need it.
  * [Digital Attack Map](www.digitalattackmap.com):  a live data visualization of DDOS attacks around the world
  * $150 can buy a week-long DDoS attack on the black market, capable of shutting down the online resources of a small organization
  * More than 2000 DDoS attacks are observed daily (world-wide)
  * 1/3 of all downtime incidents are attributed to DDoS attacks

### Distributed Denial of Service (DDoS) attacks, the basics
* If you want to take a network off the internet, the easiest way to do it is with a distributed denial of service attack.
* There are different types of attacks, but basically it means sending so much data at the site that it's overwhelmed, and not available to legitimate users
* There is an entire industry, with many technologies, devoted to DDoS defense.
* Even with an arsenal of defense, it basically comes down to a matter of bandwidth:
  * If the attacker can send more data than the defender can absorb, the website goes down and the attacker wins.



## The Internet of Things (IoT)
### What the iota huh?
* the inter-networking of physical devices, vehicles, buildings, items that exchange data
  * items embedded with electronics, software, sensors, actuators, and network connectivity that enables these objects to collect and exchange data
* The Global Standards Initiative on Internet of Things defined the IoT as "the infrastructure for the information society"
* Estimated that the IoT will consist of almost 50 billion objects by 20202

### Okay... but what are the things?
* [Crock-Pot 6-Quart. Smart Slow Cooker](http://www.crock-pot.com/slow-cookers/wemo-enabled-smart-slow-cooker/crock-pot-6-quart.-smart-slow-cooker-with-wemo/SCCPWM600-V1.html)
  * control your crock-pot from your smart phone or computer, for when you get held up and don't want to overcook dinner!
* [The 10 Best Cars with Internet connectivity](http://www.autobytel.com/car-buying-guides/features/10-best-cars-with-internet-access-130426/)
  * "Smartphones, navigation, and a stereo system are enough for the average drive. But spotty network reception can take a toll on a longer trip, leaving happy wanderers directionless and in silence, desperate to drive back into range before the kids wake up and need to stream a movie on their tablets for distraction."
* [Fitbit App](https://www.fitbit.com/app)
  * What good is a fitness tracker if you can't easily access the data it is collecting of you?
* [Five Best Smart Thermostats](http://lifehacker.com/five-best-smart-thermostats-1717145893)
  * A good thermostat can save you money on power, keep your home comfortable, even learn your habits and preferences.

* More Examples: routers, IP cameras, digital video recorders, etc...
* While these examples are consumer devices, there are also factory control devices and medical devices which send and receive information over the internet.

### Neat, what's your point?

* IoT is made of a wide range of device types, small to large, from consumer gadgets to sophisticated systems being utilized by the Department of Defense, utility and industrial/manufacturing systems.
* Due to the specialized nature of embedded systems, typical computer/ network security solutions won't even run on most embedded devices
* the majority of these embedded devices rely on simple password authentication and security protocols because it was assumed that embedded devices are not an attractive target to hackers

## They Assumed Wrong. The IoT Things are Under Attack (Hide your kids, hide your wife...)
* In late September [Krebs On Security](https://krebsonsecurity.com), a security news and investigation site, an was the target of an extremely large and unusual DDoS attack, after breaking a story that lead to the arrest of 2, 19 year old Israel men that were linked to one of the largest DDoS for hire services
* What makes this attack stand out:
  * Average peak size of a large DDoS attack at the end of 2015 was 6.88 Gbps
  * The Largest and most sophisticated typically peaked at 12 Gbps at that time
  * the attack on Krebs on Security was 620 Gbps, which according to Akamai Technologies (a DDoS protection service) was nearly twice as large as any DDoS the company had ever seen.
  * Experts noted that the size of the attack was unprecedented because it did not rely on amplification techniques and instead relied on a botnet of compromised devices (cue scary music)
    * ([DNS amplification attack](http://whatis.techtarget.com/definition/DNS-amplification-attack)) Basically, this is a popular type of DDoS that allows the data being sent out to be multiplied, so that by the time it reaches the target it is up to 100x its original size.  
  * the evidence points to a botnet comprised of IoT devices, such as routers, IP cameras, and DVRs

* a European web hosting firm, OVH, also confirmed it was hit with even more powerful DDoS attacks later that week.  
  * they made public that the attacks totaled more than 1 Tbps.
  * they discovered that the botnet behind the attack used more than 145,000 infected DVR's and Internet-connected cameras, it is believed this bot net would be capable of sending 1.5 Tbps in a DDoS attack.  




http://searchsecurity.techtarget.com/news/450305010/Powerful-DDoS-attacks-leveraging-IoT-devices-hit-several-companies

http://www.tripwire.com/state-of-security/risk-based-security-for-executives/risk-management/report-ddos-attacks-grew-in-number-size-and-sophistication-in-q4-2015/

https://www.schneier.com/

https://www.lawfareblog.com/someone-learning-how-take-down-internet

https://krebsonsecurity.com/2016/09/krebsonsecurity-hit-with-record-ddos/
