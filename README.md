## ELE306
### 25.08.22
### lære meg å bruke github
* (#) for skrift størrelse
* (*) for punkt
* CTRL V for bilder:
![image](https://user-images.githubusercontent.com/112080849/186654191-0777577d-d284-4c12-aa27-cc265cb489a4.png)
* CTRL V for videoer (maks 10mb), link for comprimering av video filer: https://www.veed.io/video-compressor?utm_campaign=YouTube+Description+Tim&utm_medium=How+to+Compress+a+Video+File+Without+Losing+Quality&utm_source=YouTube

https://user-images.githubusercontent.com/112080849/186656888-151996bf-3bfd-4e82-a9d4-5ea12d0e7743.mp4

### Hvordan vi kan code ilag ved hjelp av github:
* Trykk "code" og åpne det i visual studio. Dette er en fil som er syncet opp til github prosjektet
* Når programmet åpnes kommer dette opp (for eksempel):

![image](https://user-images.githubusercontent.com/112080849/186667268-3472e043-435b-41e4-898f-2842883f4879.png)

* Dersom jeg da vil fjerne linje 4 og synkronisere det med github prosjektet gjør vi slik:
  - Rediger det du vil redgiere:
  
  ![image](https://user-images.githubusercontent.com/112080849/186667457-841e7800-cc4f-4d8f-9b07-369cdd8b2f84.png)
  
  - Etter at noe er redigert vil blyanten nede i høyre gjørne vise at du har forandret noe:
  
  ![image](https://user-images.githubusercontent.com/112080849/186667675-9a6e72fe-9aa6-47cc-ade8-db22a86acac7.png)
  
  - Trykk deretter på blyanten og dette vinduet kommer opp:

  ![image](https://user-images.githubusercontent.com/112080849/186667831-50ae4ed5-f1ee-44ba-bb5a-f01e3eaac4f1.png)
  
  - Du trykker da på "+" for å godkjenne det du har redigert
  -Deretter kommenterer du hva du har forandret og trykket "commit":
  
  ![image](https://user-images.githubusercontent.com/112080849/186668298-be5fed61-c313-4c7c-970e-619a88c64450.png)
  
  -for og da sende det til github prosjektet, må du trykke på oppover-pilen som heter "push"
  
  ![image](https://user-images.githubusercontent.com/112080849/186668576-591fd1c3-6d1e-44b1-9342-d8bdf6b4eee1.png)
  
  
  ### 26.08.22
  ### lære meg grunleggende funksjoner av gazebo / ros
  Hadde ett stort problem med å starte gazebo. Det funket første gang, men aldri etter det. Fant løsningen.
  bruk kommandoen "gazebo --verbose", for å sjekke hva som skjer med appen, da fikk jeg beskje att den allerede kjører.
  Deretter kan vi skrive "killall gzserver". For å slå av alle gazebo prosesser.
  Note: skriv inn "gazebo" i terminalen for å starte programmet.
  
  **Kjøre en costum-world og last inn moduler fra nett **
  Første jeg prøvde var å skrive inn kommandoen "gazebo worlds/pioneer2dx.world", som i teorien skal åpne pioneer verden, dette fungerte ikke pga VM ikke fant verden
  La dette problemet på vent ettersom det sikker er en easy-fix som jeg ikke gidder å ta meg tid til nå
  
  Laste inn moduler er litt av en opplevelse. Først går vi til "http://models.gazebosim.org/"  og finner hva enn vi ønsker å importere.
  Deretter må vi gå inn i file-explorer -> home -> "model_editor_models" -> lag en mappe for det du skal importere -> legg inn .sdf og .config filene fra nettsiden.
  
  **Lage en robot i gazebo**
  Følgte en guide på youtube om hvordan å bygge en "bil" fra scratch:
  
  ![image](https://user-images.githubusercontent.com/112080849/186897017-2f245172-8d9b-4b78-846b-d00b9f13c5f8.png)

  guide som jeg følgte her:_ "https://www.youtube.com/watch?v=_qQAfTmB5wc&t=377s"
  
  ### La det forgie litt på hyllen og begynte på costum verdener
