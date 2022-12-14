<img width="600" src="https://user-images.githubusercontent.com/56886006/202922026-27fd7c5a-ceb5-4e87-bc47-2e7c14fa6a8a.png">

---

Follow me on twitter to stay updated! [Twitter @s1l1c0np1r4t3x](https://twitter.com/s1l1c0np1r4t3x)

Or get all my links here: [LinkTree @s1l1c0np1r4t3x](https://linktr.ee/s1l1c0np1r4t3)

---

# LOST AT SEA
<img width="500" src="https://user-images.githubusercontent.com/56886006/202922304-beb8c8cf-3c8d-4409-9b09-1dbc7b7e3894.png">
Link to CTF: https://hacktoria.com/contracts/lost-at-sea/

## Description/Debrief

Greetings Special Agent K. Yesterday at exactly 22:34 EET we lost contact with our surveillance ship “Narwhal”. A distress signal was sent out, right after this all communication was lost. The Narwhal was operating in the Black Sea, keeping an eye on Russian submarine and aerial activity.

Although she looks like a regular fishing trawler, the Narwhal, built in 2018, was outfitted with state of the art equipment. Housing a crew of 10, including a 4 PAX intervention unit of our best and brightest from the H.M.I.U (Hacktoria Maritime Intervention Unit).

Our allies in the British Royal Navy were kind enough to respond immediately. They were able to retrieve the Narwhals’ distress beacon. This is a device that automatically logs the last ten event, using the many sensors on board. This quick log entry is written to the SD card inside a waterproof tube, outfitted with a flotation device and GPS beacon. After the data is written, the beacon ejects and keeps afloat on the surface.

This prevents any signal delay from external antennas not being fast enough. Now, there’s a catch with this beacon. The log-file is written to an encrypted archive. The password for this log-file is set by the captain and communicated over encrypted channels, changing daily to prevent enemy forces capturing the correct code.

Somehow, the signal was lost right before the captain was able to relay the new password. This is human error, the password would normally be communicated right before being changed. This leaves us with our current situation. We don’t know the password, you’ll have to find a way to unlock the log-file.

This will give us insight into how the Narwhal sunk and allow us to begin the recovery. Given the hostile situation, it’s imperative we find the exact location of the Narwhal.


---

## Process:

The objective is to obtain access to a password protected file that is the logbook of the ship and will reveal its last location.
<br/>

### 1. Download assets
**Downloaded ship logbook file**

  
<img width="500" src="https://user-images.githubusercontent.com/56886006/202922659-1ecf0c1a-806e-4ec8-8d95-2175e38d8564.png">
As you can see the logfile is indeed password protected.
<br/>
  
**Before I dove in an put the file up against software like Hashcat, John the Ripper, etc., I decided to try and crack the password myself with a little social engineering.**


### 2. Analyze the information given in the debrief
**What do I know?**
<ul>
  <li>Lost contact with the ship yesterday at exactly 22:34 EET.</li>
  <li>The Narwhal was operating in the Black Sea.</li>
  <li>It's mission was to keep an eye on Russian submarine and aerial activity.</li>
  <li>The ships name is the Narwhal.</li>
  <li>The ship was built in 2018.</li>
  <li>Looks like a regular fishing trawler.</li>
  <li>It is outfitted with state of the art equipment.</li>
  <li>Houses a crew of 10.</li>
  <li>British Royal Navy responded immediately.</li>
  <li>General beacon technology overview.</li>
  <li>General Captain password proticol overview.</li>
</ul>


**What sticks out?**
<ul>
  <li>Operating in the black sea.</li>
  <li>The ships name (The Narwhal).</li>
  <li>The ships build date (2018).</li>
  <li>The ship resembles a regular fishing trawler.</li>
</ul>

**Going off the information that stuck out to me I decided to try the most basic passwords I could think of given the information I know as well as the information that stuck out to me.**


### 2. Attempt password combinations with given information
**Password attempts in order:**
<ul>
  <li>narwhal</li>
  <li>Narwhal</li>
  <li>narwhal2018</li>
  <li>Narwhal2018</li>
</ul>

## SUCCESS!

<img width="500" src="https://user-images.githubusercontent.com/56886006/203345010-7a5e4673-6a16-43b2-8690-2596086750a6.png">

On the fourth attempt the logfile was unlocked and I was able to access the information needed.

While this one was extremely easy and guessed on only the fourth attempt, not all will be this easy. I was easily expecting to go into different combinations of using the current AO "the black sea" and the type of vessel theirs looked like "a fishing trawler." 


h4ppy hunt1ng!

s1l1c0np1r4t3
