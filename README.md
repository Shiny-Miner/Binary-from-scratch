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
# Level 1 : Patching , advance level patching and bit on what they do and ALL INFO on offsets and bytes for a start!
Probably if your a good pokemon player then you should be allready knowing why patches are made but lets take this topic to advance level.
Hmm whenever you've been roaming around in some often used communities like Pokeconmunity and try to download a rom hack and its in attachments but --- in some unknown .ips,.ups,.bps format? Ah sus i wanted a .gba rom man!
## What are these patches? Why do rom hackers create them?
The patch (ips/bps/ups) is an incredible formot which keeps us away from having copyright strikes from game freak or nintendo. Sharing .gba rom files is not allowed (try to share them anywhere in public and they will ban you)
It better to be on safer side! Agree?
But i left ```Actually what it does?``` 
So to understand this you need to know about hexadecimal system.
Hexadecimal system or hex in simple language is basic block of our rom or i can say the binary language (after zeroes and ones). It just like a mixed counting with Numbers and alphabets till F.
So really what we humans use is simple number system is called 
decimal system when comparing with hexadecimal system. 0,1,2,3,4,5,6,7,8,9 right but what after it? 10? No! in hexadecimal system after 9 We give place to 'A' then 'B' , then 'C' then 'D' then 'E' and then 'F' and then comes 10.
So basically We're adding 6 new numbers while going from zero to ten in hexadecimal counting. Consider A,B,C,D,E,F as numbers as they're as important as 1-9.
### Q. What will be our decimal number 30 in hexadecimal language?
So you may try a bit more and you will understand it well. You can look in more examples like our 16 is 10 in hex. Our 255 is FF in hex, and so on...
#### What was the need?
Now you'll understand things a bit more clearly, now you know our Pokemon Fire red rom? It is of 16 MB and it contains hexadecimal numbers from 0 to FFFFFF. A lot isn't it? And actually here's a bit tricky point those all hex numbers are actually some type of address or place where 2 Numbers are stored. What i mean is like suppose you go to address FFFFFF and there you met 2 people and that's it. An hex address cannot have less or more than two people in it. And we refer these hex addresses as 'Offsets' and the 2 people living there are called bytes. Every byte contains important data for rom and as all hex address or offsets are continuous in numbers so are the bytes. The Bytes or 2 people living at that house if both are 00 or FF (bytes also follow hex rule) then its a free space inside rom.
Suppose we go to offset BD302 and we found bytes there as 'FF' then its a free offset. I'll tell you more about free offsets in later of this tutorial. Now let's move to what patches do.
#### Patches on a Pro level!
Every operation we do in our rom, we're changing these bytes, sometimes replacing some (very usual), sometimes freeing up some (rare), even adding graphics, maps, scripts all just do byte changes in your rom and these bytes are changed in a way that we can actually get our desired output. Well what patches do is comparing these bytes changes, saving a data file like .ips which contains data, at this offset this bytes was changed and when applied to a vanilla/clean rom the magic happens.
BUT, this isn't enough, while making a patch you're asked for 2 roms one is modified rom and one is original rom (unmodified) but its not necessary that your unmodified rom should be a vanilla rom. I mean suppose you added a trainer card and made a patch then it will be a trainer card patch but if you do the reverse? What i mean is if you would have taken the modified trainer card rom as unmodified rom in your patch creator and vanilla rom as modified rom then IT WILL BE A REMOVAL PATCH!
That's all about advanced level. Surely read this 1-2 times more and you'll never forget about offsets and bytes they're the necessary elements if you want to be a good rom hacker (we're gonna do some cool bytes changes in next Level so that you get to know how dynamic byte changes can be)

# Level 2 Finding a FR rom and unzipping
Probably this is my github and I'm not gonna care of anyone else. I SHARE you the link to the best and cleanest Fire Red rom I'm using till now... 
[Link](https://archive.org/download/1636PokemonFireRedUSquirrels/1636%20-%20Pokemon%20Fire%20Red%20%28U%29%28Squirrels%29.zip/)
Now what you gonna need is Winrar , the best tools to play with these unzipping and so things. We need this thing 500 times a day lol.
Probably lemme share a premium version of WinRar for Free
https://blindhelp.net/software/winrar
Click the Download for windows button to download it and install it , well all pokemon fans know these things so I leave this till here. For those who don't know , just install this winrar and now right click on your .zip file (test on the rom zip) and then click Extract to < archive name > something like this just click it and the file be in now in a folder thats it.
#### Remember in later tutorials or if you're a hex maniac advance user Opening zip file in Hex maniac doesn't works so you need to follow it first!!!
