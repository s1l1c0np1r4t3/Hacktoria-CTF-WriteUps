<img width="600" src="https://user-images.githubusercontent.com/56886006/202922026-27fd7c5a-ceb5-4e87-bc47-2e7c14fa6a8a.png">

---

Follow me on twitter to stay updated! [Twitter @s1l1c0np1r4t3x](https://twitter.com/s1l1c0np1r4t3x)

Or get all my links here: [LinkTree @s1l1c0np1r4t3x](https://linktr.ee/s1l1c0np1r4t3)

---

# The Butcher
<img width="500" src="https://user-images.githubusercontent.com/56886006/205346761-4e96b0e1-1181-4128-b769-ac9709b2dbf6.jpg">
Link to CTF: https://hacktoria.com/contracts/nightmare-fuel/

## Description/Debrief

Greetings Special Agent K. Yesterday evening around 2100 hours, two officers of the New York Police Department entered the premise of an abandoned building in Brownsville New York. Neighbors had complained about strange sightings. Supposedly a woman had been squatting inside the building.

Reports also state that over the course of the two years the building has been abandoned, several residents of the surrounding houses had complained about junkies occupying the building. Often making terrible screeching like noises during the night.

Normally, this would not get the attention of the NYPD, however, a neighbors’ security camera had caught several people entering the building, but never seen them emerge. Upon closer inspection, a neighbor reported that all windows were closed and intact. Her security camera had also been on the whole time, surveying the only entrance to the building.

This eventually got the NYPD to investigate the building. While clearing rooms, the officers noticed someone moving around at the end of a hallway. Upon repeated calls and commands, the individual retreated behind a door. Both officers approached the door and told the person to come out. After a few seconds, we could see a woman move past the door frame.

Unresponsive to any commands given by the officers, they continued their search. Never to find the woman again. The officers called for backup and had a team of twelve officers and a K-9 unit sweep the building.

Nobody was ever found. Even the dog didn’t find a trail. Which is odd, given all the smells clearly lingering around an old building like that. Strangely enough, upon inspecting the body cam footage, the audio appeared to be missing entirely.

We need you to take a look at the video and see what you can find.

As always, Special Agent K, the contract is yours. If your choose to accept.

---

## Process:

The objective is analyze the body camera footage from the officer and attempt to discover any information that might useful.

### 1. Analyze the information given in the debrief
**What do I know?**
<ul>
  <li>Body camera footage from an NYPD officer needs to be analyzed for information.</li>
</ul>

This is the body cam footage from the officer:

<img width="500" src="https://user-images.githubusercontent.com/56886006/205346939-30ee3186-267f-457f-a8a3-317d9461c00b.gif">

Creepy huh?

Let's see if we can't find anything about the video that might be useful.

The first think I noticed was the audio was indeed missing. There was no audio to the video. 

I decided to run it the video through my favorite metadata tool exiftool:

https://github.com/exiftool/exiftool

https://exiftool.org/



Here is the command I used:

`exiftool bodycam-officer-1.mp4` 

Through the use of exiftool you can learn all sorts of things about videos and pictures. It is a great tool that runs on Windows, Linux and Mac. Not only that but it has a stand alone available so no install is needed on some platforms.

Some might think only pictures have metadata and videos do not. But that is not true, videos have metadata available in them the same as pictures do. Even offering up infromation about frame rates and volume.

Here are the results:

<img width="500" src="https://user-images.githubusercontent.com/56886006/205347233-9b270edb-d777-4a7d-8c9a-0f0e9cd2c6c2.png">

As you can see there was a lot of information got looked for and was available.  

However one thing specifically sticks out if you know what you are looking for. In the metadata of any video or picture there is a comment option. This is usually blank unless changed by a person or a piece of software. Curios enough to have a look at it, at least for me.

<img width="500" src="https://user-images.githubusercontent.com/56886006/205347393-62245440-da4b-4011-baeb-eb6af5ac3cd0.png">

It is an odd string of letters and numbers.

I decided use this seemingly random string of letters and numbers to try and open the Hacktoria flagfile.

<img width="500" src="https://user-images.githubusercontent.com/56886006/205347768-8853b489-3427-4fc4-92f1-b78450ee9857.png">

SUCCESS!!

The string of letters and numbers found in the comment area of the videos metadata gave us the correct password to be able to open the Hacktoria flagfile, get out sweet contract card and claim victory over this CTF!


h4ppy hunt1ng!

s1l1c0np1r4t3
