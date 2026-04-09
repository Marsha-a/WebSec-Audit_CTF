Raport z testów bezpieczeństwa: Aplikacja webowa CTF-1

**Autor:** Marsha
**Data wykonania:** 05.03.2026 - 10.03.2026
**Metodyka:** OWASP TOP10, OWASP ASVS
**Podejście:** Black Box & Grey Box
**Wykorzystane narzędzia:** Burp Suite Community, ffuf, Nikto, nmap

Podsumowanie audytu
Testy bezpieczeństwa wykazały obecność 7 podatności o różnym stopniu krytyczności. Identyfikacja luk pozwoliła na odnalezienie ścieżki eskalacji prowadzącej od ujawnienia kodu źródłowego do pełnego przejęcia kontroli nad systemem poprzez zdalne wykonanie kodu.

##Zidentyfikowane podatności

* **[CRITICAL]** CTF-1-001: Wyciek kodu źródłowego poprzez Local File Inclusion (PHP Wrappers)
* **[CRITICAL]** CTF-1-002: Remote Code Execution (RCE) poprzez błędy w obsłudze plików i LFI
* **[HIGH]** CTF-1-003: Domyślne dane uwierzytelniające w publicznej dokumentacji
* **[HIGH]** CTF-1-004: Domyślne dane uwierzytelniające i podatność na ataki typu Brute-force
* **[MEDIUM]** CTF-1-005: Brak serwerowej weryfikacji żądań Cross-Site (CSRF)
* **[LOW]** CTF-1-006: Ujawnienie wrażliwych zasobów w pliku robots.txt
* **[INFO]** CTF-1-007: Podatność na enumerację wirtualnych hostów

---
*Szczegółowe techniczne dowody koncepcji (Proof of Concept) oraz rekomendacje naprawcze dla każdego ze zgłoszeń znajdują się w dokumencie PDF.*
