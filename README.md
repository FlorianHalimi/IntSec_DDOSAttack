# IntSec_DDOSAttack
Zhvillimi i një aplikacioni që mundëson DDOS attack dhe kundrejt firewalleve dhe proxyve si cloudflare

DDoS sulmi qëndron shkurt për "Distributed Denial-of-Service" dhe është një sulm kibernetik në të cilin sulmuesi përmbyt një web server me kërkesa të shumta të gjeneruara vetë, në mënyrë që një përdorues i vërtetë të mos ketë mundësi të qaset dhe të marrë shërbimet e nevojshme nga ky web server pasiqë web serveri nuk është më i aftë të pranojë kërkesa. 
DDoS sulmi ndodh nga paisje të shumta të shpërndara në Internet, për dallim prej DoS i cili përdor një burim të vetëm për të sulmuar sistemin. 

Cloudflare përdoret për minimizimin e sulmeve  DDOS, mirëpo nuk është shumë i sigurtë.

Ky aplikacion mund të sulmojë faqet të cilat janë dhe nuk janë të mbrojtura nga sistemi mbrojtës Cloudflare.

Komandat ndihmëse: 



Përmes:
--help - mund të shohim të gjitha komandat
--host - përcaktojmë faqen në të cilën inciojmë sulmin
-d     - path-in e faqes
--ssl  - HTTP/HTTPS
--port - Porti psh. 80/443
-t     - numri i thread-ave
-x     - proxy fajll-i


Në rastin e parë, kur sistemi është i mbrojtur nga Cloudflare:
Komanda për të filluar sulmin është : python DDOS.py --host cloudflare.com --ssl -x proxy-list.txt



Ne rastin e dytë, kur sistemi nuk është i mbrojtur nga Cloudflare:
Komanda për të filluar sulmin është : python DDOS.py --host kompjuterika.tk



Numri default i threads është 100, mirëpo nëse dëshirojme ta ndërrojmë mundemi përmes komandës -t:

