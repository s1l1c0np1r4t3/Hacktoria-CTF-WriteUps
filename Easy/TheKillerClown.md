<img width="600" src="https://user-images.githubusercontent.com/56886006/202922026-27fd7c5a-ceb5-4e87-bc47-2e7c14fa6a8a.png">

---

Follow me on twitter to stay updated! [Twitter @s1l1c0np1r4t3x](https://twitter.com/s1l1c0np1r4t3x)

---

# THE KILLER CLOWN
<img width="500" src="https://user-images.githubusercontent.com/56886006/203387508-b85a5f71-bd9f-4384-8271-a7b448edba2e.png">
Link to CTF: https://hacktoria.com/contracts/the-killer-clown/

## Description/Debrief

Greetings, Special Agent K. We have a very urgent case on our hands. The San Francisco Police Department is working on a true horror case this October. There is an actual killer clown roaming the streets of the greater San Francisco area.

The killer is dressed as a clown and strikes at night, mostly targeting women and younger men. The victims are drugged and bound tightly with a long rope, stretching all the way around the body. After this, the killer attaches an oxygen tank to the victim and puts them inside a coffin sized box. Making it impossible to move, but just enough to breathe slowly.

The victim is then buried alive and a picture is taken of the location, which is then sent to the police. With the amount of oxygen in the tank, victims usually last about 24 hours. Though with the panic setting in, some die within 6 hours. A few others suffered a heart attack from the panic. They are left as a game, for the police to find the location in time, or not. So far there have been several sightings of a clown at night, though only for brief moments. In one of the photo’s, the image of the clown was visible in a car mirror caught on camera.

About 30 minutes ago, the San Francisco Police Department received a new picture from the clown. This time we have reason to believe the victim is Melany Parker, a 23 year old woman from Northwest Berkeley. She was reported missing by her boyfriend, after she didn’t return from her evening jog.

Given the circumstances, we have no time to waste. Your assignment is simple, find the location of the picture below. Before the next victim dies, tied up in a box underground, slowly suffocating while tightly wrapped in ropes.

Special Agent K. The contract is yours, if you choose to accept.


---

## Process:

The objective is to put together the password to a file in which contains the location of the victim using the current location of the victim  discoverable only through a picture provided by the suspect. (Pictured directly below.)

<img width="500" src="https://user-images.githubusercontent.com/56886006/203388747-2f92d2cd-02e6-43e7-8670-3e1d2fd170b6.jpg">


### 1. Download assets
**Download Linkfile**

<img width="500" src="https://user-images.githubusercontent.com/56886006/203388951-254dcbbd-214c-4adc-a7ea-c924db54dafb.png">


The file is indeed password protected. A sample password was supplied: 

> Sample password, no caps: local-park-name-dirty-mud-path

**Instead of trying to crack the password or anything like that I decided to dive right in and try to find the location of the victim using the image provided.**


### 2. Analyze the information given in the debrief
**What do I know?**
(Focusing specifically on the victim to expediate her rescue)
<ul>
  <li>The victim is Melany Parker.</li>
  <li>23 year old woman.</li>
  <li>From Northwest Berkeley.</li>
  <li>San Francisco area.</li>
  <li>Reported missing by her boyfriend.</li>
  <li>She didn’t return from her evening jog.</li>
</ul>


### 3. Get a lay of the land
Using strictly the information about the current victim I headed to good ol' google maps to get a better idea of the area our victim was last seen.

This is the general area of the attacks as well as our current victim.

<img width="500" src="https://user-images.githubusercontent.com/56886006/203389895-e0615745-1469-4f71-8cb9-568108e8e9b4.png">

I immediately noticed Berkeley on the map as the are where the victim is from. So I decided to take a closer look there.

<img width="500" src="https://user-images.githubusercontent.com/56886006/203390200-e2e014a7-827a-4f61-b748-0790cc0b9a05.png">
<img width="500" src="https://user-images.githubusercontent.com/56886006/203390158-434db564-caf9-4c71-915c-a34092fb241e.png">

The victim was reported missing by her boyfriend after not returning from her evening jog.

While the possibilites of the victims route if very large I wanted to stick with the most likely of possibilites. I decided to look for trails or parks which someone might go jogging. Specifically in the Northwest region of Berkley.

<img width="500" src="https://user-images.githubusercontent.com/56886006/203390403-6ea7700b-0de9-4846-a1f9-8bce64c4c8a3.png">


### 4. Narrow down and search the more likely places a jogger would be abducted

As you can see in the North West vacinity of Berkely where are victim was abducted there are 2 main parks where the victim might have been jogging. 

<img width="500" src="https://user-images.githubusercontent.com/56886006/203390626-15f85935-bf66-4329-9ce2-70502fefe9ca.png">

I decided to start with Cedar Rose Park as it is the closest to the North West area on the map. 

<img width="500" src="https://user-images.githubusercontent.com/56886006/203390725-a85f190c-cc19-46b4-8c79-a8da9eba960b.png">

Looking back at the picture we notice a few things to look for in the park where the victim is located:

<ul>
  <li>Paved (black tar) walkways</li>
  <li>Bench+Trashcan on walkway</li>
  <li>Building or house behind bench/walkway.</li>
  <li>Noted tree and brush possibly overgrown near site.</li>
  <li>Noted shape of walkway, opens up on the side for bench/trashcan</li>
</ul>

<img width="500" src="https://user-images.githubusercontent.com/56886006/203391014-3b6f6941-f9e5-48c6-8694-17c0d3b6de5e.jpg">

Looking at the first park Cedar Rose 

I noticed the walkways, trashcan and bench in one of the google maps photos about 10 pictures down was the same as the one in photo supplied by the suspect. I made a mental note that is possible these trash cans are standard from the city or state and could be in many of the parks in the area. But I felt like this was a good start and definately at least warranted a closer look.

<img width="500" src="https://user-images.githubusercontent.com/56886006/203391234-dde7f515-9cc8-41f5-9803-8cf7ecd60c07.png">

I took note of the where the picture was taken by the uploader from the little yellow avatar that represents google street view. So I backed out of pictures and looked for that spot on maps.

<img width="500" src="https://user-images.githubusercontent.com/56886006/203391494-561098dd-c3f1-4383-8e6e-39504b87fd33.png">

Although that didn't work (google marked where the picture was taken wrong), I decided to take the google maps street view avatar to each entrence of the park to see if I noticed anything. On the 4th one I came across this:

<img width="500" src="https://user-images.githubusercontent.com/56886006/203391645-e1ec6741-14c0-4ead-8dee-4367ab6ebb0f.png">

Notice these few things:

<ul>
  <li>The bench, pole and trash can all match.</li>
  <li>The pole and trashcan are both to the right of the bench.</li>
  <li>The pathway matches as well as the enclove for the bench on the path.</li>
  <li>The tree looks similiar to the one in the picture as well as the bush underneath it.</li>
  <li>There seems to be the possibility of a small clearing behind the bench.</li>
  <li>Brown building set back away from the bench area.</li>
</ul>

<img width="500" src="https://user-images.githubusercontent.com/56886006/203391967-75b309e1-9ea2-46b7-a0db-4d2669cf85d4.png">

This looked like a very promising possibility to me. Knowing I needed the park name and the path name for the password I noted the park name was "Cedar Rose Park" and started to look for the path name.

There was no signs or paths name availabe from street so I back to normal view to see if it wasn't marked on the map.

On this photo I marked the location of the street view, bench and building. As well as I circled the name of the path "Ohlone Greenway."

<img width="500" src="https://user-images.githubusercontent.com/56886006/203392134-26afa722-1071-4029-b0f0-6dd6c52d1a98.png">

Now I have the name of a park and pathway in that park that seems like a very good possibility to try asthe password for the file supplied by the suspect. Cedar Rose Park, Ohlone Greenway.

Sample password, no caps: local-park-name-dirty-mud-path

local-park-name = cedar-rose-park
dirty-mud-path = ohlone-greenway

cedar-rose-park-ohlone-greenway 
 
SUCCESS!

It would seem that I foudn the corret location! Using the name of the correct park and pathway combined as outlined in the sample password, I was able to unlock the file and retrieve the flag!

<img width="500" src="https://user-images.githubusercontent.com/56886006/203392345-20c9ccc9-feb9-4148-b625-840545a4e6e4.png">

This one was fun. I did stop some where in the middle to look at other parks in the area. I spent maybe 15mins just going real quick in between as many in the area as I could to see them at least visually. 

Until next time!
