<img width="600" src="https://user-images.githubusercontent.com/56886006/202922026-27fd7c5a-ceb5-4e87-bc47-2e7c14fa6a8a.png">

---

Follow me on twitter to stay updated! [Twitter @s1l1c0np1r4t3x](https://twitter.com/s1l1c0np1r4t3x)

---

# LOST AT SEA
<img width="500" src="https://user-images.githubusercontent.com/56886006/202922304-beb8c8cf-3c8d-4409-9b09-1dbc7b7e3894.png">
Link to CTF: Link to CTF: https://hacktoria.com/contracts/lost-at-sea/

---

## Process:

The objective is to obtain access to a password protected file that is the logbook of the ship and will reveal its last location.
<br>

### 1. Download assets
**Downloaded ship logbook file**

  
<img width="500" src="https://user-images.githubusercontent.com/56886006/202922659-1ecf0c1a-806e-4ec8-8d95-2175e38d8564.png">
As you can see the logfile is indeed password protected.
<br>
  
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

<img width="500" src="https://user-images.githubusercontent.com/56886006/202923399-09681078-a703-4952-ae89-ba1f86e0020f.png">

On the fourth attempt the logfile was unlocked and I was able to access the information needed.

While this one was extremely easy and guessed on only the fourth attempt, not all will be this easy. I was easily expecting to go into different combinations of using the current AO "the black sea" and the type of vessel theirs looked like "a fishing trawler." 
