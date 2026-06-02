Acest
repo
a
fost
creat
pentru
a
documenta
proiectul
cursului
de
Printare
si
Modelare
3D

<h1>Cinematograf</h1>
<p>În cadrul acestui proiect, voi modela un videoproiector pentru film </br> Acest mecanism constă într-o manetă ce rotește niște gears, transformând o rotație într-o oscilație verticală pentru a muta un cadru cu o furcă ce avansează filmul la o anumită viteză și un obturator.</p>

<h2>Surse de inspirație</h2>
<a href="https://en.wikipedia.org/wiki/Cinematograph">Cinematograf Lumiere</a>

<h2>Proces</h2>
<p>Pentru a putea reda o versiune funcțională a mecanismului a trebuit să studiez în profunzime ansamblul de mecanisme ce îl alcătuiesc și să calculez cu atenție și precizie parametrii acestora. Am citit și manuale de matematică și tot nu am înțeles ce dimensiuni ar trebui să îi dau de fapt (https://books.google.ro/books?id=U9eOPjmaH90C&pg=PA83&redir_esc=y#v=onepage&q&f=false !!!nu imi zice cu cat il deplaseaza!!!).</p> 
<p>Am crezut că i-am dat de cap excentricului triunhiular, dar realizând joint-urile, am observat că îmi mișca doar la jumătate din distanța dorită, așa că am ajuns la concluzia că trebuie să îl dublez, dar după ce am făcut asta și am refăcut și cadrul și joint-urile nu se mai mișca deloc cum trebuia, halucina tare!! Am găsit un site care calculează parametrii pentru excentric și parametrii mei erau halucinați se pare? dar tot nu am înțeles cum trb făcut și efectul pe care îl are excentricitatea, căci site-ul calcula pentru orificiu central, deci iar ar fi trebuit să refac și este foarte târziu și trebuie să învăț la rețele și Radu nu răspunde pe Teams :( (ar fi amuzant să răspundă cât scriu asta :D)</p>

<p>Presupunând că mânerul e rotit de două ori pe secundă trebuie să îi transmitem rotația axului central pe care stau toate componentele noastre care depind de rotație. Vrem 16fps (la 24 erau prea mari pinionii și trebuia să refac cutia și nu mai încăpea pe bed-ul imprimantei). O rotație completă a axului principal ne dă ciclul unui cadru, deci la 16 cadre și 2 rotiri ne trebuie de 8 ori mai multe, deci small gear cu 10 dinți modul 1 și big gear 80 dinți modul 1 să nu fie prea mare și nici cea mică prea mică...of</p>

<h1 style="danger">Problem!!!</h1>
<p>Furca mea ce prinde filmul trebuie să se miște sus-jos și față-spate și nu știu cum să fazez aceste mișcări, sus-jos o mișcă excentricul cu cadrul, dar față spate îmi trebuie un cylindrical cam și nu știu ce parametrii să dau șanțului pentru că nu știu cât timp ar trebui să îmi ia in-out, up-down și cert e că NU SE ÎNTÂMPLĂ SIMULTAN CELE DOUĂ TIPURI DE MIȘCĂRI. Și nici excentricul nu mai înțeleg câte sus-jos îmi dă într-un ciclu 2 sau 3 ;-; </p> 
<p>Am zis să obturez 90 de grade din 360, adică o pătrime de ciclu, dar pare cam mult că, în timpul obturației coboară filmul și cât e expus iese furca, urcă și intră, dar dacă coboară 90 atunci urcă 90 si e in si e out tot cate 90, poate ar trebui mai puțin?</p>

<h2>Concluzii</h2>
<p>Mă gândesc prea mult, cred că doar trebuia să implementez dar nu știu exact și mă deranjează că nu pot vizualiza corect și deduce răspunsul. Am găsit o chestie pe thingiverse, dar nu e funcțională, e doar pentru expunerea principiului, deci NU ARE PARAMETRII PE CARE MĂ CHINUI DE DOUĂ ZILE SĂ ÎI DEDUC CORECT >((((</p>
<p>Nu am motion study, nu am render, poate pun gcode-ul la componentele parțiale pe care le am. Probabil că nu voi trece, dar oricum e vina mea că am avut o lună la dispoziție.</p>
<p>Ar fi trebuit să le împart pe foldere înainte să pun aici...direct pe main...</p>
<p>Dar ca să închei într-o notă pozitivă, poate termin până la 23:59 :D</p>

<h2>Resurse</h2>
<ul>
  <li>https://books.google.ro/books?id=U9eOPjmaH90C&pg=PA83&redir_esc=y#v=onepage&q&f=false</li>
  <li>https://youtu.be/IrhOnLc-awQ?si=pH1WtPQkJfc1S_We</li>
  <li>https://www.thingiverse.com/thing:1557789/makes</li>
</ul>
