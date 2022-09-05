# ELE306


## GITHUB


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
  <br/>
  <br/>
  <br/>
  <br/>
  <br/>
  ## ROS / GAZEBO
  
  
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
  Hvordan å launce f.eks. turtlebot3:
  
  ![image](https://user-images.githubusercontent.com/112080849/186930925-64a66525-260b-4a4a-ac99-c112a4672269.png)

  Deretter kan vi også f.eks. åpne ett nytt terminal vindu for å styre roboten:
  
  ![image](https://user-images.githubusercontent.com/112080849/186931320-bda7f4dd-f424-4a03-8ef7-37935eabc7a0.png)



  https://user-images.githubusercontent.com/112080849/186932850-ff752d45-3947-46d1-b155-87f615d882a2.mp4
  
  <br/>
  <br/>
  <br/>
  <br/>
  <br/>
  
  ## Universal robots
  
  
  ### 26.08.22
  ### laste ned og forstå grunnleggende elementar av simulering av robot arm
  
  Har VMware fra ROS delen, dermed kan vi bara laste ned operativ systemet som Universal robot selv har lagt ut
  
  Windows versjon:  
  https://www.universal-robots.com/download/software-cb-series/simulator-non-linux/offline-simulator-cb-series-non-linux-ursim-3158/
  Linux versjon:    
  https://www.universal-robots.com/download/software-cb-series/simulator-linux/offline-simulator-cb3-linux-ursim-3158/ 
  
  Importer den inn i VMware og godta / ignorer alle errors / meldinger!
  
  ![image](https://user-images.githubusercontent.com/112080849/186993941-8cb272da-7e64-4c14-8788-14875914e602.png)

  har fått meg inn på simulatoren, men sliter med å sette opp ett 3D område for å kunne teste ting med robot-armen.
  
  ## Simulering i matlab
  
  Bruk D* navigerings script fra Cork robotics som eksempel.
  step 1: Fin fil-mappen f.eks. (C:\Users\joaki\AppData\Roaming\MathWorks\MATLAB Add-Ons\Toolboxes\Robotics Toolbox for MATLAB\demos).
  step 2: åpne filen som heter det du ønsker å simulere (f.eks. dstarnav.m)
  da vil matlab se slik ut:
  ![image](https://user-images.githubusercontent.com/112080849/188493601-c2133907-a44c-4dee-8bf6-d7ae4c25e8cc.png)
  step 3: skriv inn "rtbdemo" i kommand vinduet og trykk "D* navigation".
  step 4: dersom vi ønsker å forandre på forskjellige ting, kan vi kjøre det ved å redigere ".m" filen. Vi kan forandre start punkt, veridene til forskjellige celler
  osv.
