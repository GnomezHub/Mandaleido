# Mandaleido
## Final project on my fullstack developer course @Lexicon
#### The idea is to make a web adaptation of my actionscript air application "Mandaleido", that uses controls to make kaleidoscopic animations of an image provided by the user.

[![Demo Video](https://github.com/user-attachments/assets/812290e0-21d6-4cd2-b45c-db57f3729182)](https://www.youtube.com/watch?v=V7Cxf1Wduok)
**_click the screenshot image to watch a video demo_**

It will have a database to store the animation presets and images, with different roles.

---

_Fortsätter på svenska, översätter till engelska i ett senare skede_

Mandaleido är ett program som jag skrev för att projicera det på fester, på taken i chillout-tälten mest. Man drag& droppar bilder så animeras dom. Ändrar de olika parametrarna med skrollhjulet. Olika fönster, så att man kunde ha effekterna på fullskärm i em separat skärm projicerad.
Det här projektet går ut på att göra en webb-adaptering av det över 10 årig gamla programmet. Inte för projektioner nödvändigtvis, kanske mer för sin meditativa effekt, eller för att ta fram mandala liknande mönster av egna bilder...

Det ska gå att:
- testa lagrade presets, ändra dessa (temporärt) och välja bland uppladdade bilder om man är anonym. 
- skapa och lagra och ställa in presets samt att lägga upp bilder, om man är inloggad.
- allt ovanstående samt ta bort och lägga till bilder och presets oavsett vems, om man är admin (inloggade kan göra detta enbart på sina egna)

I den första fasen försöker jag ta fram en webb baserad version av de kaleidoskopiska animeringar. 

I den andra fasen skapar jag kontrollerna för att styra och ställa in parametrarna.

Den tredje och kanske största fasen är inloggning& registrering, bilduppladdning och gränsnittet för att lista de olika presets, samt skapa& ändra och ta bort bland dessa.

I den fjärde fasen snyggar jag till alltihopa och finns det tid över så lägger jag till features som bildgenerering, som även fanns i originalet. Och kanske anpassning till fullscreen.
Finns det ännu mer tid över så gör jag mobilversion av kontrollerna, och nyttjar mobilens olika sensorer till att ändra parametrarna.

----

Jag har på kvällen testat att översätta det jag gjorde i flash till js, och kommit fram till att det kommer att ta längre tid än jag trodde att få den effekt jag söker. Så jag har tänkt kasta om prioriteringarna, så att jag i första fas gör en oath baserad inloggning med usertabell i supabase databas.

---

Valet stod mellan MVC och react&supabase. Med MVC skulle jag ha fått mycket gratis då jag redan har gjort en grund med inloggning, användare med roller och bilduppladdning när jag gjorde filmdatabasen. Men det blev react och supabase då jag behöver utmaningen att göra om detta på det 'andra sättet' som dessutom möjliggör att potentiella arbetsgivare kan testa mitt slutprojekt online utan installeringar. Vidare lämpar sig react för denna webbapplikationen som bör ligga på en sida utan omladdningar.
