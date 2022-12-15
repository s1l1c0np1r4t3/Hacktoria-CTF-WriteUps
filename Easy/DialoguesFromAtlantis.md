<img width="600" src="https://user-images.githubusercontent.com/56886006/202922026-27fd7c5a-ceb5-4e87-bc47-2e7c14fa6a8a.png">

---

Follow me on twitter to stay updated! [Twitter @s1l1c0np1r4t3x](https://twitter.com/s1l1c0np1r4t3x)

Or get all my links here: [LinkTree @s1l1c0np1r4t3x](https://linktr.ee/s1l1c0np1r4t3)

---

# Dialogues from Atlantis

<img width="500" src="https://user-images.githubusercontent.com/56886006/207939789-90849499-30ed-4d2c-b6bf-f4b229967e07.jpg">

https://hacktoria.com/contracts/dialogues-from-atlantis/


## Description/Debrief

Greetings, Special Agent K. One of our clients, a wealthy art collector from Monaco, is requesting we help her find a recorded dialogue between Critias, Hermocrates, Timaeus and Soscrates.

In her quest to unravel the mysteries regarding the ancient city of Atlantis, our client wishes to gather all evidence possible as to where the location of the lost city truly is. Getting stuck a fair bit into her endeavors, she has reached out to Hacktoria to decipher a piece of text.

Our client believes this text to be of vital importance to prove the existence of Atlantis as a city. Whether it will lead directly to the discovery of the city is doubtful. Nonetheless, it’s of great importance to unravel its meaning.

I trust your ability to deal with ciphers and ancient dialogues in this matter. You find the text below. In the end, this will lead to another Contract Card if you manage to complete this assignment.

As always. Special Agent K, the contract is yours, if you choose to accept.

---


## Process:

The objective is to help try and find a recorded dialogue. We have to decipher a piece of text. Successfully deciphering the text correctly will give us the password we need to unlock the flagfile, get our contract card and mark this challenge complete.

### 1. Analyze the information given in the debrief
**What do I know?**
<ul>
<li>Text needs to be deciphered.</li>
  <li>Correctly deciphering the text will give us the ability to unlock the flagfile.</li>
</ul>

This is an image of the text:

<img width="500" src="https://user-images.githubusercontent.com/56886006/207939867-9a55a59e-2d9a-40c5-92e5-120a10c03d23.png">

We can instantly recognise this is a HEX code.

So I headed over to https://gchq.github.io/CyberChef/ to start investigating.

<img width="500" src="https://user-images.githubusercontent.com/56886006/207939918-295e504e-037e-41c7-a3d8-7a7c2b892b12.png">

Use the From Hex option.

<img width="500" src="https://user-images.githubusercontent.com/56886006/207941367-a4b5ee7b-e3e5-437b-8726-aadad07e2548.png">

When we bake that bad boy this is what we get:

<img width="500" src="https://user-images.githubusercontent.com/56886006/207941438-c23a9878-c681-4b7f-a388-1ec23639a069.png">

<img width="500" src="https://user-images.githubusercontent.com/56886006/207941496-84e8f226-850d-46ae-9858-22c4193228cd.png">

Not recognizing the encoding type off hand I played around a little in CyberChef and even tried to use the magic option but with no luck.

<img width="500" src="https://user-images.githubusercontent.com/56886006/207941554-90679553-245c-4107-a123-790a2f7237a5.png">

I decided to take this weird text to https://dencode.com/en/

I ran this text through all of the options, ALL, string, date, color, cypher, hash.

<img width="500" src="https://user-images.githubusercontent.com/56886006/207941605-dc3ccae3-3188-4e1b-98b8-990afb8a6552.png">

<img width="500" src="https://user-images.githubusercontent.com/56886006/207941659-4da0a640-d38f-497a-897a-6a502dc68c9a.png">

<img width="500" src="https://user-images.githubusercontent.com/56886006/207941696-71103a5a-499c-4c4e-a52c-4acfa8928541.png">

On the cipher option something stuck out to me that was the same as when I searched all. While all other encoding types spit out similar code as one another, except ROT47

<img width="500" src="https://user-images.githubusercontent.com/56886006/207941744-d6ca5064-ff9b-46f3-a5de-9132e4b087c6.png">

This discrepancy leads me to believe this type may have returned a unique value maybe because it is being used.

I headed back to CyberChef to do some cooking.

I added ROT47 to my CyberChef recipe.

<img width="500" src="https://user-images.githubusercontent.com/56886006/207941790-df2afc80-3073-467e-b5d7-357bddafe03b.png">

Once again we get a different set of text. This one happens to look like Base64 however! I'm hoping this is another encoded type that I can spot at this point, but with this challenge I am ready to pivot again.

Let's try adding Base64 to the recipe.

WOAH! It looks like we got some readable text as output!

<img width="500" src="https://user-images.githubusercontent.com/56886006/207941834-2749ae4f-c102-47e9-8c05-778d22b96301.png">

Here is a better picture of the text:

<img width="500" src="https://user-images.githubusercontent.com/56886006/207941883-dce11c1b-d88d-4332-907c-9413445b1d8f.png">

I was unsure of what to do with this text now so I made sure to read it a few times. On my third read through I noticed a discrepancy in the text.

<img width="500" src="https://user-images.githubusercontent.com/56886006/207941921-d0bac32e-6cf4-485a-b230-defad8025df5.png">

It kind of looks like a bit link (a shortened link)

Shortly after I also realized I had missed this twice.

<img width="500" src="https://user-images.githubusercontent.com/56886006/207941977-0a81cbe3-a6a8-4d30-b0d2-000d11d98aa2.png">

I put the two together and decided to try them in my web browser.

But no luck. The links are broken.

Finally I decided to try the link as the password to the flagfile.

<img width="500" src="https://user-images.githubusercontent.com/56886006/207942019-668edffb-ea85-4656-9e52-48d0015289d5.png">


After trying for 30 minutes to unlock the wrong flagfile with this password I put together. I selected the correct flagfile and was able to successfully retrieve the contract card. 

Had lots of fun with this one and I love the story and lore.


h4ppy hunt1ng!

s1l1c0np1r4t3
