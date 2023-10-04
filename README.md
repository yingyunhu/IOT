# IOT - Philips Hue
Ying Yun Hu

# 1. Adafruit installeren
1. Als allereerst installeer ik de Adafruit library.

<img width="274" alt="Screenshot 2023-10-04 at 12 55 51" src="https://github.com/yingyunhu/IOT/assets/112943865/4339ba65-fedd-41b4-8d64-05b532f8fd51">

2. Oh! Ik moet eventjes de andere library ook downloaden om deze library te kunnen gebruiken. Ik klik op 'Install all'. 
<img width="548" alt="Screenshot 2023-10-04 at 12 56 17" src="https://github.com/yingyunhu/IOT/assets/112943865/bca2fc0e-7c36-48a8-a014-05ec2afa96b3">

3. Gelukt!

<img width="326" alt="Screenshot 2023-10-04 at 12 57 06" src="https://github.com/yingyunhu/IOT/assets/112943865/8196ce1b-89ea-4d57-8b1b-095238d2d620">

# 2. Nu gaan we beginnen met de setup van Adafruit IO. Ik maak een account aan. 
<img width="1470" alt="Screenshot 2023-10-04 at 13 00 25" src="https://github.com/yingyunhu/IOT/assets/112943865/505d26e1-fa1f-4469-b960-f4d57843c120">

1. Even de gele sleutel aanklikken zodat ik mijn key en gebruikersnaam kan kopieëren.
<img width="228" alt="Screenshot 2023-10-04 at 13 06 00" src="https://github.com/yingyunhu/IOT/assets/112943865/f76b05e9-0c06-49e5-a003-4bfbf14f9426">

# 3. Colorpicker

1. Nu ga ik een nieuwe dashboard aanmaken voor de color picker. 
<img width="1408" alt="Screenshot 2023-10-04 at 13 09 00" src="https://github.com/yingyunhu/IOT/assets/112943865/45b05db8-2be9-42c3-aaf8-cae5a57786c8">

2. Een nieuwe block aanmaken en deze connecten met een nieuwe feed die ik 'color' heb genoemd.
<img width="790" alt="Screenshot 2023-10-04 at 13 11 51" src="https://github.com/yingyunhu/IOT/assets/112943865/a8803df4-7904-4b7d-ac4c-304f8f58278e">
<img width="777" alt="Screenshot 2023-10-04 at 13 13 46" src="https://github.com/yingyunhu/IOT/assets/112943865/268cd633-ba64-41bd-ad6e-58679132071a">

3. Eventjes een leuke roze tint uitkiezen voor m'n colorpicker! Hoppa. 

<img width="450" alt="Screenshot 2023-10-04 at 13 18 01" src="https://github.com/yingyunhu/IOT/assets/112943865/e31a7d8b-ef41-42d1-adfb-1278adf47304">

<img width="443" alt="Screenshot 2023-10-04 at 13 14 38" src="https://github.com/yingyunhu/IOT/assets/112943865/75c7c154-1a4b-4ff0-813b-c9f4c8e09c0d">

# 4. Code aanpassen in Arduino
1. Oh, ik moest Adafruit OI Arduino nog installeren volgens het word document, want deze stond nog niet bij examples. Dit ga ik snel even doen.
<img width="329" alt="Screenshot 2023-10-04 at 13 24 15" src="https://github.com/yingyunhu/IOT/assets/112943865/70d5cc4e-f280-4e80-aa5f-4c877de7e529">

<img width="215" alt="Screenshot 2023-10-04 at 13 21 52" src="https://github.com/yingyunhu/IOT/assets/112943865/ff356f80-9a65-48e1-af1e-03d5e5066774">

2. Alllllll deze libraries installeren. 
<img width="584" alt="Screenshot 2023-10-04 at 13 23 01" src="https://github.com/yingyunhu/IOT/assets/112943865/0daac25a-ed88-47b8-8e0c-ee1d4c6b6d7d">

3. Hij staat er nu bij! Nu naar File > Examples > Adafruit IO Arduino > Adafruitio_14_neopixel. 
<img width="691" alt="Screenshot 2023-10-04 at 13 26 19" src="https://github.com/yingyunhu/IOT/assets/112943865/61dc9862-3de8-4ef0-a5ef-993f15f43df5">

4. In config.h mijn gebruikersnaam, key, wifi netwerk (mijn hotspot in dit geval) en wachtwoord invoeren in de code.  
<img width="678" alt="Screenshot 2023-10-04 at 13 31 20" src="https://github.com/yingyunhu/IOT/assets/112943865/63e1d3e8-e100-4751-bb17-7dae457c91ff">

5. in de Tab adafruit_14_Neopixel.ino de #define PIXEL_PIN 5 aanpassen naar #define PIXEL_PIN D5.
<img width="309" alt="Screenshot 2023-10-04 at 15 19 40" src="https://github.com/yingyunhu/IOT/assets/112943865/406abfac-4841-4d69-9ac3-af8a28071eb5">

# 5. Code uploaden
1. Eerst verifyen en dan uploaden. Geen erros yay!
<img width="962" alt="Screenshot 2023-10-04 at 13 35 45" src="https://github.com/yingyunhu/IOT/assets/112943865/74c967c0-62ca-4b2b-b533-6edbb74d84bd">

2. De serial monitor activeren. Deze op 115200 baud zetten. 
<img width="161" alt="Screenshot 2023-10-04 at 13 37 59" src="https://github.com/yingyunhu/IOT/assets/112943865/815c63db-807c-423a-9981-86e8d43d86aa">

3. Hij hoort nu verbonden te zijn... Maar hij geeft ondeindig stipjes aan....
<img width="927" alt="Screenshot 2023-10-04 at 13 40 25" src="https://github.com/yingyunhu/IOT/assets/112943865/18437cb0-a6e3-4e9b-8872-6343fc0a784d">

4. M'n led strip is uitgegaan.. Maar het lichtje brandt nog wel op het bord. 
<img width="200" alt="Screenshot 2023-10-04 at 13 40 25" src="https://github.com/yingyunhu/IOT/assets/112943865/ca742a91-3153-4831-b25f-ea4f7bc81124">
<img width="200" alt="Screenshot 2023-10-04 at 13 40 25" src="https://github.com/yingyunhu/IOT/assets/112943865/6dd04cde-a573-4ac0-a1be-ea66b6b1d40f">

5. Misschien de naam aanpassen van m'n hotspot? Dus niet de IP adres invullen maar de naam van m'n hotspot. 
<img width="252" alt="Screenshot 2023-10-04 at 14 50 22" src="https://github.com/yingyunhu/IOT/assets/112943865/643c7fb9-846b-4058-8b24-15935d1ab185">

Nope. 

<img width="200" src="https://github.com/yingyunhu/IOT/assets/112943865/4c443bbe-5fd0-4533-a355-6d3539a659f8">

6. Ligt het aan m'n hotspot instellingen?
<img width="676" alt="Screenshot 2023-10-04 at 15 58 10" src="https://github.com/yingyunhu/IOT/assets/112943865/d524748f-09c0-419d-ae8b-3378588960ab">

Zucht.. Deze stond al aan. 

<img width="200" src="https://github.com/yingyunhu/IOT/assets/112943865/6bf78957-4926-4f16-b4f3-3ac8e2243f93">


8. De naam van m'n dashboard misschien veranderen naar 'color'? 
<img width="681" alt="Screenshot 2023-10-04 at 14 59 18" src="https://github.com/yingyunhu/IOT/assets/112943865/5f699d1a-b258-4e00-8432-5c52c11b974e">

Nope, heb nog steeds de puntjes. 
<img width="926" alt="Screenshot 2023-10-04 at 15 09 48" src="https://github.com/yingyunhu/IOT/assets/112943865/fce204ed-21e0-4550-8206-da6875b175ab">

Ik heb nu over verschillende mogelijke problemen gedacht, maar helaas werkt de led strip nog steeds niet als het moet. Dit kan waarschijnlijk aan mijn hotspot/wifi liggen? 
Ik heb m'n medestudenten gevraagd of zij misschien kunnen helpen, maar ook zij kwamen niet achter het probleem. Wel alsnog gek omdat de code geen errors aangeeft, dus het hoort wel gewoon te werken :( Het installeren van Adafruit ging super soepel, dus jammer dat m'n serial motor als laatste stap niet wilt verbinden. 




