# Where all it starts!
Let's start this amazing documentation based on a noob 3 yr rom hacker experience.
The one who used to play with PGE (Pokemon Game Editor), G3HS (Gen 3 Hacking Suite) and G3T (Gen 3 Tools) started playing with Advance map , HxD, XSE and then 
started to play with Decomps, CFRU, and Hex Maniac. Broke more than 100 roms, made resources. Fine right? Ok, consider this as my intro.
I don't want you to follow my path but just want to tell you a bit : DO NOT TRUST HELP FROM DISCORD.
Actually instead of asking for help from people i helped people. Can you think a person who only knows how to play with PGE helps people (though wrong but something sounding fun?)
This improved my vision. I poured out hours not in asking help but to bringing out my ideas, i broke 1 rom worked again and again, even through a copy paste made script (probably experimenting every script i found on pokecommunity) i made this : https://www.pokecommunity.com/threads/the-most-awaited-buying-pokemon-script-for-gba.456390/

Ignore caps, i was a noob named Luke111 trying to spam and thought caps made your text more clearer xD.

So PEOPLE are you ready to climbing this hurdle? ROM Hacking is nothing but trust in yourself more than others. Break things and make experiments instead of being a slave of already made creeps make your own creep.
##### Ignore all the tool names and things i shared above if you know nothing about them
REFER these question and answers for some clarity : https://github.com/Shiny-Miner/GBA-Binary-hacking-assets/wiki/Information-about-binary-:-A-start
# Level 1 : Patching , advance kevel patching and bit on what they do.
Probably if your a good pokemon player then you should be allready knowing why patches are made but lets take this topic to advance level.
Hmm whenever you've been roaming around in some often used communities like Pokeconmunity and try to download a rom hack and its in attachments but --- in some unknown .ips,.ups,.bps format? Ah sus i wanted a .gba rom man!
## What are these patches? Why do rom hackers create them?
The patch (ips/bps/ups) is an incredible formot which keeps us away from having copyright strikes from game freak or nintendo. Sharing .gba rom files is not allowed (try to share them anywhere in public and they will ban you)
It better to be on safer side! Agree?
But i left ```Actuslly what it does?``` 
So to understand this you need to know about hexadecimal system.
Hexadecimal system or hex in simple language is basic block of our rom or i can say the binary language (after zeroes and ones). It just like a mixed counting with Numbers and alphabets till F.
So really what we humans use is simple number system is called 
decimal system when comparing with hexadecimal system. 0,1,2,3,4,5,6,7,8,9 right but what after it? 10? No! in hexadecimal system after 9 We give place to 'A' then 'B' , then 'C' then 'D' then 'E' and then 'F' and then comes 10.
So basically We're uding adding 6 new numbers while going from zero to ten in hexadecimal counting. Consider A,B,C,D,E,F as numbers as they're as important as 1-9.
### Q. What will be our decimal number 30 in hexadecimal language?
So you may try a bit more and you will understand it well. You can look in more examples like our 16 is 10 in hex. Our 255 is FF in hex, and so on...
#### What was the need?
Now you'll understand things a bit more clearly, now you know our Pokemon Fire red rom? It is of 16 MB and it contains hexadecimal numbers from 0 to FFFFFF. A lot isn't it? And actually here's a bit tricky point those all hex numbers are actually some type of address or place where 2 Numbers are stored. What i mean is like suppose you go to address FFFFFF and there you met 2 people and that's it. An hex address cannot have less or northan two people in it. And we refer these hex addresses as 'Offsets' and the 2 people living there are called bytes. Every byte contains important data for rom and as all hex address or offsets are continuous in numbers so are the bytes. The Bytes or 2 people living at that house if both are 00 or FF (bytes also follow hex rule) then its a free space inside rom.
Suppose we go to offset BD302 and we found bytes there as 'FF' then its a free offset. I'll tell you more about free offsets in later of this tutorial. Now let's move to what patches do.
