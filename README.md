Ez a projekt egy statikus HTML alapú weboldal, amely több HTML fájlt és képeket tartalmaz.
A cél a biztonságos böngészés és a lehetséges veszélyek felismerése és védekezés ellenük, emellett weboldal konténerizálása Docker segítségével, hogy bárhol, bármilyen környezetben könnyen futtatható legyen.
A projekt Nginx webszervert használ a statikus fájlok kiszolgálására.

A projekt klónozásához és verziókezeléséhez szükséges egy GitHub Desktop.
Telepítés után:
-Jelentkezz be GitHub fiókoddal
-Klónozd a repót a gépedre

A konténer építéséhez és futtatásához szükséges a Docker Desktop.
Telepítés után:
-Engedélyezd a WSL2 backend használatát
-Indítsd el a Docker Desktopot
-Várd meg, amíg az állapot: Docker is running
Ellenőrzés: docker version parancs.

Docker image buildelése
A projekt mappájában futtasd:
" docker build -t biztonsag-web " parancsot.
Ez létrehozza a biztonsag-web nevű Docker image‑et.
Ezután a " docker run -d -p 8080:80 biztonsag-web " parancs segítségével futtassa a konténert, majd a http://localhost:8080 oldlaon megtekintheti az oldalt.
