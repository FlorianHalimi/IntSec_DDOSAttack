# IntSec_DDOSAttack
Zhvillimi i një aplikacioni që mundëson DDOS attack dhe kundrejt firewalleve dhe proxyve si cloudflare

DDoS sulmi qëndron shkurt për "Distributed Denial-of-Service" dhe është një sulm kibernetik në të cilin sulmuesi përmbyt një web server me kërkesa të shumta të gjeneruara vetë, në mënyrë që një përdorues i vërtetë të mos ketë mundësi të qaset dhe të marrë shërbimet e nevojshme nga ky web server pasiqë web serveri nuk është më i aftë të pranojë kërkesa. 
DDoS sulmi ndodh nga paisje të shumta të shpërndara në Internet, për dallim prej DoS i cili përdor një burim të vetëm për të sulmuar sistemin. 

Cloudflare përdoret për minimizimin e sulmeve  DDOS, mirëpo nuk është shumë i sigurtë.

Ky aplikacion mund të sulmojë faqet të cilat janë dhe nuk janë të mbrojtura nga sistemi mbrojtës Cloudflare.

Komandat ndihmëse: </br></br>
![help](https://user-images.githubusercontent.com/74669741/148700939-1f1a1275-e4bf-4108-b6fe-198bffa66c8a.png)

Përmes:</br>
--help - mund të shohim të gjitha komandat</br>
--host - përcaktojmë faqen në të cilën inciojmë sulmin</br>
-d     - path-in e faqes</br>
--ssl  - HTTP/HTTPS</br>
--port - Porti psh. 80/443</br>
-t     - numri i thread-ave</br>
-x     - proxy fajll-i</br>


Në rastin e parë, kur sistemi është i mbrojtur nga Cloudflare:
Komanda për të filluar sulmin është : python DDOS.py --host cloudflare.com --ssl -x proxy-list.txt

![2](https://user-images.githubusercontent.com/74669741/148700964-e4f00f09-58a1-4fbb-8365-48e5d386d9a3.png)

Ne rastin e dytë, kur sistemi nuk është i mbrojtur nga Cloudflare:
Komanda për të filluar sulmin është : python DDOS.py --host kompjuterika.tk

![1](https://user-images.githubusercontent.com/74669741/148700969-f46881a8-b2ab-42dd-ae9f-74c0241a33b8.png)


Numri default i threads është 100, mirëpo nëse dëshirojme ta ndërrojmë mundemi përmes komandës -t:</br>
![2 1](https://user-images.githubusercontent.com/74669741/148700973-5097fa08-70dd-429b-ad59-5bb9318ee4d9.png)


