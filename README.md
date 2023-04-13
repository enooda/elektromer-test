# elektromer-test
Kód je napísaný v Jave pre Selenium Webdriver. Test sa vykonáva pomocou metódy  validaciaElektromera()", ktorá sa spúšťa pred každým behom testu v rámci triedy "elektromerTest". V metóde "setUp()" sú inicializované premenné a vytvorené zoznamy. V metóde "validaciaElektromera()" generujú náhodné údaje pre jednotlivé parametre a vyhodnocuje sa ich vierohodnosť.
<br></br>
**Logika:**
<br></br>
Ak je spotreba rovná 0, zaznamená sa. Ak sa tak stane viac ako "x" krát po sebe a ak uplynulo aspoň "y" dní od posledného merania, a ak nie je dôvod odpočtu alebo druh odpočtu rovný určitým hodnotám, údaje nie sú považované za vierohodné a premenná "isValid" sa nastaví na false. V opačnom prípade sa považujú za vierohodné a premenná "isValid" sa nastaví na true.
<br></br>
<ul>
<li>Test prebehne iba v prípade, že je validácia zapnutá</li>
validationOn = true
<li>Pre získanie viacerých dát na validáciu je cyklus nastavený na 15 opakovaní</li>
<li>Výpočet dní, ktoré uplynuli medzi odpočtami je nastavený ako aktuálny dátum – náhodný dátum do 1 roka. Výsledok sa uloží ako "pocetDniInt"</li>
<li>Druh odpočtu a dôvod odpočtu sú definované ako ArrayList, z ktorých sa vyberá náhodná hodnota "druhodpoctuValue" a "dovododpoctuValue"</li>
<li>Ako aktuálny stav elektromera a predchádzajúci stav elektromera sú dosadené náhodné čísla medzi 100 a 2 000</li>
</ul>
