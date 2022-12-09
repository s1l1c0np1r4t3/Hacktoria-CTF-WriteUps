<img width="600" src="https://user-images.githubusercontent.com/56886006/202922026-27fd7c5a-ceb5-4e87-bc47-2e7c14fa6a8a.png">

---

Follow me on twitter to stay updated! [Twitter @s1l1c0np1r4t3x](https://twitter.com/s1l1c0np1r4t3x)

Or get all my links here: [LinkTree @s1l1c0np1r4t3x](https://linktr.ee/s1l1c0np1r4t3)

---

# The Butcher
<img width="500" src="https://user-images.githubusercontent.com/56886006/206763236-94322bc7-4df7-428d-aab4-d9ba73871849.jpg">
Link to CTF: https://hacktoria.com/contracts/the-butcher/

## Description/Debrief

Greetings, Special Agent K. As you might have heard in the news over the past few months. The city of Berlin in Germany is being plagued by a serial killer, nicknamed “The Butcher”.

As the name implies, this individual butchers his victims and disposes their body parts all over the city. Autopsy reports conclude that the weapon for disposal is most likely a meat cleaver.

The total body count currently sits at 18 people, mostly women and younger men. All victims were traveling alone at night, mostly through quiet areas, when they were last seen.

Fortunately, yesterday the German police raided an apartment in the city center of Berlin. Neighbors had complained about a stale, metal like smell coming from the apartment. Upon closer inspection, the police found large quantities of plastic sheets, blood traces of several victims and an assortment of meat cleavers.

Since the apartment was rented out to an individual who had used a fake ID, the police has hit a dead end in trying to find the killer. They did however retrieve several files from a personal laptop, including a large, encrypted archive.

In the same location as the archive was stored, a file named “password” was found. However, this just contained a bunch of HEX values. We need you to make sense of this file, perhaps it leads to the password for the archive.

As always, Special Agent K. The contract is yours, if you choose to accept.

---

## Process:

The objective is to gain access to the encrypted archive by using a file stored on the device labeled "password". We must make sense of this file and return with a usable password for the encrypted archive.


### 1. Analyze the information given in the debrief
**What do I know?**
<ul>
  <li>A file named “password” was found.</li>
  <li>It is an encrypted archive</li>
  <li>Contained HEX values.</li>
</ul>

This is a picture of the HEX values that come up when you open the file:

<img width="500" src="https://user-images.githubusercontent.com/56886006/206763330-0c075c51-30d7-469a-8651-22ca3a9e521e.png">

Pull the file from Hacktoria to better be able to work with it.

`wget https://hacktoria.com/wp-content/contracts/items/password-the-butcher`

<img width="500" src="https://user-images.githubusercontent.com/56886006/206763415-406896ca-46b1-482c-a6d2-200cf4f81b0e.png">

Now the that we have the file downloaded and ready to investigate, what would be our next step?

We need to try and make sense of this HEX code to be able to unlock the file. 

There isn't much out there better than CyberChef. I had the pleasure of doing a deep dive into CyberChef thanks to TryHackMe's Advent of Cyber this year. CyberChef is a truely amazing tool. I've been using it since 2018. It is dubbed "The Cyber Swiss Army Knife." And for good reason! 

CyberChef can be used to: Encode, Decode, Format data, Parse data, Encrypt, Decrypt, Compress data, Extract data, perform arithmetic functions against data, defang data, and many other functions.

It is a go to and a must know for all cyber security enthusiests!

CyberChef has a live version from one of their repos on github. 

https://gchq.github.io/CyberChef/


Open the file in CyberChef. We want from HEX.

<img width="500" src="https://user-images.githubusercontent.com/56886006/206763486-8ef585c4-e1e8-4c68-9ac8-fc5b20c6d70c.png">

It looks like a bunch of nonsense information but if a great feature of CyberChef is the detect file type. 

<img width="500" src="https://user-images.githubusercontent.com/56886006/206763621-190088c7-abf3-4848-8de7-bccccf7db5c0.png">

And we get an mp3 file type. We know know this is an mp3 audio file.

<img width="500" src="https://user-images.githubusercontent.com/56886006/206763692-ad6328d1-275e-464c-a931-de24b8bddb19.png">

Select save file, and when you save it make sure to give it proper file name extension since it is a mp3 file. Example: `theButcherAudioFile.mp3`

<img width="500" src="https://user-images.githubusercontent.com/56886006/206763737-339def68-2277-4c2d-9e78-799860022739.png">

Open VLC player and import the audio file into it. 

<img width="500" src="https://user-images.githubusercontent.com/56886006/206763775-5749f727-616d-4b89-a4b2-bb6bf049f8dc.png">

Hit play. 

There is a voice that says a bunch of characters. Write these down.

Enter those characters into the Hacktoria flagfile. 

<img width="500" src="https://user-images.githubusercontent.com/56886006/206763813-0db77eb1-4354-4854-941d-20a253e54c7c.png">

SUCCESS!

We have successfully decoded the HEX file, save it to its intended format, and found a way to use that format to get the password to the flag file through sound.


h4ppy hunt1ng!

s1l1c0np1r4t3
