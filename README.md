# Pallet-1.0
This Is a Releases only repository made exclusively to be an outlet for downloading the Pallet 1.0 tool, for information on Pallet please read the ReadMe.txt where you can find usage instructions, current bugs, learning goals and expected and unexpected learning results. 

# Overall Learning Outcome:
this project was mostly to keep my development skills warm after graduation, i had an idea of a tool that could be useful to creators like myself who have a nack for art and creative hobby's. i also wanted to try out WFP a desktop app framework in c#, my most previous experience before developing this application was a REACT RESTful API web site which was all about encrypting user data and their documents and acting as a sort of third party for PPI to block companies selling users data, so i wanted something morel light and fun. another goal of mine was to make the database simple, i used a txt document for it, and it is layed out like: colourName, HEX. ie:

Dim Red,#C05060
Karry,#FFECD3
Atomic Tangerine,#FEA465
Crusta,#FC7643
Apple Blossom,#AF4F41
Pickled Bluewood,#273148

and there is another one txt document for pallettes, but the goal is you just have to do into the data folder in the applications folder where its app data exists and replace the text document with your own one, effectively allowing easy simple data transfer, you could change your whole library easily, and you could even ask generative ai to write you a library, just write a prompt like "could you produce 50 colours in this format: colourName, HEX and example would be: Dim Red,#C05060." and you have a whole new set of colours.

# things i liked about WFP:
wfp was different but also felt familiar, the way the UI elements syntax worked reminded me of html but still different, the styling did feel clunky and also make the code feel busy visually, if you're going for a visual masterpiece then i probably wouldn't use wfp and when i plan to re do this project i will probably use something else. any ways this section is called what i LIKE about wfp not what i hate so.
- i liked how lightweight the app is, its exe is only 148 kb but its folder is more like 150mb, which sounds like alot but compared to other frameworks like REACT which can be giga bytes i think its decent, can't get much more lightweight than this without a minimalist framework
- i liked being able to write  the backend in c# and not having to use any IPC to communicate with the backend


# Known Bugs:
there is some known bugs which A. i didn't know existed until i published this app and or B. i didnt feel the need to fix it as i plan to reapproach this app and make it something near perfect, 
- truncating of text - in the libraries of the colours and pallettes (this visual bug i knew of before i released, i figured it wasn't very important and in a more polished version i will be more motivated to make it look cleaner)
- Fixed screenshot, now this ones a big one - and is the result of poor testing. when i wrote this app i used my fixed screen resolution...(i know very bad) and completely forgot to make it system based, so unless you screen resolution is the same as mine when i wrote this application, you will likely have part of the screen missing when you try to select/pick a colour. this could of been simply avoided if i had tried the software on another device before releasing on github and could be fixed in a couple mins but... i will re work this project so i figured its fine as this is really early days for this concept

# Challenges: 
the biggest challenge of this project was figuring out the picking functionality, we needed to make it feel seemless, so how it works is, when we click pick, the app takes a screenshot and displays it in the palet window, but it makes  the screen view fullscreen without the title bar giving the illusion that their screen is frozen in time, then we had to write from scratch a cursor which was a scope showing the individual pixels that the cusor was over. writting the cursor tracking and reprinting of the cursor was probably the most difficult part but the challenge was fun and i probably could of found some kind of a library in the nuGet but then there wouldn't be much learning other than the framework for this project. 
