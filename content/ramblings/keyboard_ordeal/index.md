---
title: "Keyboard Ordeal"
date: 2023-12-05T16:18:16+02:00
tags: ["keyboard", "split", "dhl", "splitkb.com"]
---

## Backstory

I have been avid watcher of [Ben Wallack](https://www.youtube.com/@BenVallack) for quite while, especially all the keyboard stuff he has done over the years. Not sure what made me make up my mind, but month ago I finally decided to get small and ergonomic keyboard.
So I did what anyone would do and reseached the options for solid week scrolling through all the possible keyboard options and stores to buy them ([very cool website for that](https://kbd.news/vendors/split)).
I wanted to get prebuilt keyboard to not mess anything up since all the options were expensive. My optios were Dygma Defy, UHKv2 and zsa voyager but all of them would've costed me about 450€ which was way over budget, and they didn't exactly fit my needs either.
The absolute cheapest way would've been to order the boards directly from JLPCB with everything soldered on, which I did consider, but that approach was cheap only if you ordered multiple and sold some to your friends for example since you could only order in bulk.
Getting the boards directly from pcb manufacturer also meant that I would've had to go fully caseless or get 3d printed case for extra cost. I then stumbled on splitkb.com who sold kits in eu and had excellent documentation, support and reputation.
I was able to get full kit with nice premium looking and feeling case for only 200€ which was pretty good (the absolute cheapest set I could gather for the aurora sweep in there was around 140€).

## Shopping

I had decided on where to buy and what to buy. I went trough the nice kit composer which added every part needed easily to my cart (except keycaps). I was super excited so I only glanced over the cart for having everything and just pressed buy.
I got asked what shipping option I wanted: all of them said 3-5 days so I picked the cheapest DHL option, it can't be that bad right? (it was that bad).
Two days go by and I realized that I didn't order any homing keys (the keys with small nobs on them for index fingers to find their location). I also read in their discord server that they would be stocking the keycaps, that I had picked, in white color, which I wanted much more, but were out of stock when ordering.
I then contacted the support and asked if they could've added one pair of homing keys and switch the color of my ordered caps to white. They answered in a day and said that they could add the homing keys but the keycaps would arrive later that week and asked whether I wanted to put the order on hold until they arrived or send the order immediately.
I really wanted those white caps so I answered that they should wait one week for the caps, and if they didn't arrive by then, to just send the order as is. They did exactly that and shipped it next monday with white caps.

## Shipping

I got the tracking code into my email and started following it, checking every hour or so for updates. First it left the store (located in netherlands) and got moved to DHL's sorting center in germany.
This was all good and dandy but everything went wrong the next day when it was reported to have been arrived in the destination country, but that destination country was UK for some reason.
I emailed the seller and got response basically telling to be patient (which was fair since it had only been there for one day). I emailed DHL and they said that only the seller could start investigation.
I even emailed Royal Mail and they said that they could not do anything since I wasn't the sender but they did confirm that they had the package and didn't know why it wasn't being handled in any way.
So I did the only thing I could do at that point, waited. I waited for around two weeks and messaged the seller again and this time getting response telling how they told DHL to start investigating the package.

![Nice 20 day jump](/ramblings/keyboard_ordeal/history.png)\
_20 days of nothing, was probably sitting in UK customs waiting for someone to pay_

## Customs

The reason I went to great lenghts in finding the store in eu was to avoid dealing with customs so I was highly amused when I got message telling that I should pay the duty/vat to receive my package which arrived from outside eu.
I then called the customs to explain the situation and the response I got was that it would be the responsibility of the postal service to release it from the customs. I checked the postal service's website, tried to call them, failed because the number is paid and my number could no call to those, and started a chat with some agent using their website.
The agent was polite and nice but denied everything the customs call had said and instead told me that it would've been illegal for anyone but the customs to release the package. This was totally false and anyone could confirm it easily, but I couldn't change the agent's mind.
I then called using another phone and another agent asked for some document to prove the origin country of the purchase. I sent the document and the package got released the next day. It then took one day to arrive at "a" pick up point, had to drive 10km to pick it up.
This so called 3-5 day shipping was from 7th of November to 1st of December, whopping 24 days! You can guess how pleased I was (and currently am) with DHL globalmail. The seller had been very nice and responsive the whole time so this was purely DHL being garbage company.

![Illegal to release](/ramblings/keyboard_ordeal/customs.png)\
_Message from postal service agent telling me how only the customs can release packages stuck in customs_

## Assembly

Assembling the kit was very straight forward. All the instructions were super clear and soldering wasn't as hard as it first had seemed to be. Took me 5-6 hours to fully assemble everything.
Only mistake I made was breaking off one header leg from one of the controllers which I was able to fix by replacing it with diode leg.

![Parts](/ramblings/keyboard_ordeal/parts.jpg)\
_All the parts came in nice zip bags_

![Broken off leg](/ramblings/keyboard_ordeal/leg.jpg)\
_One of the header legs broke off when I pulled the controller of the sockets too hard_

## Software

Once I had built the keyboard it was time for installing and customizing the firmware. I use Fedora Silverblue as my operating system of choice so I thought setting up the QMK environment would be easy. I painstakingly installed all the dependencies which were no listed anywhere (later found install script with all the necessary package names from the qmk repo), but I just couldn't get it to compile any firmware for my microcontroller. I also tried the docker approach but that failed with different errors. I happen to be bit of a gamer so I also have windows installed and was able to set up the environment there succesfully.
I then used the next 8 hours trying to get some kind of layout together and reading the QMK documentation on how stuff worked and barely got alpha layer working in that time (alphas are the basic letters). It took another day for there to be enough layout to fully start using it.
I have since edited the layout daily bit by bit small changes when I need or think of something. Here's repo containing the layout in it's current state [repo](https://github.com/luimu64/qmk_layouts/tree/master/sweep).

## Closing thoughts

I have been using the keyboard now for couple days and it has been exactly what I had hoped for: small, ergonomic, effective and cool looking. Only small issues I've had are the cable I picked being too short and switches being bit too heavy both of which are easy and cheap to fix.
The biggest takeaway in this whole dealing is to use DHL express for stuff you actually care about arriving even if it costs bit more. It's worth it, trust me.

![Finally done](/ramblings/keyboard_ordeal/done.jpg)
