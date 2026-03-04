Szkolenie: "Dlaczego hackowanie aplikacji webowych jest proste? Przegląd najnowszych/najciekawszych luk bezpieczeństwa w aplikacjach"

Autor: Michał Sajdak, Sekurak

Szkolenie prezentowało rzeczywiste podatności w aplikacjach webowych (SSRF, RCE, SQL Injection, błędy autoryzacji i resetu haseł) oraz ich konsekwencje. Omówiono przypadki z realnych systemów i odniesiono je do klasyfikacji OWASP Top 10. Szkolenie pozwoliło zrozumieć mechanizmy najczęstszych ataków na aplikacje webowe oraz znaczenie prawidłowej kontroli dostępu i walidacji danych wejściowych.

Spis treści:

1) Aplikacja AI do analizowania dokumentów i pomocy w wygrywaniu przetargów firmy Minerva:
   - bezpośrednio poprzez przeglądarkę można było dostać się do listy użytkowników oraz konwersacji z chatem AI
   - można było również uzyskać dostęp do poufnych dokumentów

2) Aplikacja FlowiseAi do tworzenia agentów AI:
   - podająć adres e-mail dowolnego użytkownika w funkcji resetu hasła można było zresetować mu hasło i dostać się na jego konto
  
3) Aplikacja AI dla prawników FileVine:
   - odwołanie w komunikacji http do zasobu na AWS, w odpowiedzi można było uzyskać uwierzytelnienie dla pełnego administratora
  
4) Aplikacja McDelivery w Indiach:
   - możliwość zmiany wartości koszyka i zamówienia jedzenia prawie za darmo
  
5) Oprogramowanie McHire:
   - poprzez login i hasło 123456 można było dostać się do panelu administratora testowej restauracji McDonald's oraz uzyskać dostęp do rozmów kandydatów ubiegających się o pracę

6) Aplikacja Subaru:
   - ominięcie 2FA, łatwy reset hasła w ukrytym panelu logowania i dostęp do aplikacji, gdzie można było poznać lokalizację samochodów

7) Aplikacja Gitlab:
   - bardzo podobna podatność do FlowiseAI, możliwość resetu hasła użytkownikowi i włamania na konto

8) Biblioteka React, framework Next.js:
   - niebezpieczny exploit pozwalający na dostęp do wrażliwych danych po stronie serwera
   - podatne były wszystkie aplikacje używające React
   - hackerzy bardzo często kopali kryptowaluty na serwerach lub włączali je do botnetu

9) TinyBox - serwery VPS:
   - podatność umożliwiająca dostęp do bazy danych
   - możliwość tworzenia za darmo wirtualnych serwerów
   - kod aplikacji TinyBox został wygenerowany w 100% przez AI i nie uwzględnił ważnych aspektów bezpieczeństwa

10) Aplikacje Triofox i Confluence:
   - podatność umożliwiająca stworzenie więcej niż jednego administratora

11) King addons for Elementor - plugin Wordpress:
   - możliwość stworzenia nowego użytkownika z uprawnieniami administratora całkowicie anonimowo

12) Internetowe konto pacjenta:
   - poprzez modyfikację adresu URL można było uzyskać dokumentacje medyczne innych pacjentów

13) Wielkopolskie Centrum Medycyny Pracy:
   - ta sama podatność co w IKP

14) Platforma HackerOne:
   - poprzez modyfikację id w adresie url można było uzyskać dostęp do raportów audytów bezpieczeństwa innych aplikacji

15) Aplikacja F1:
   - możliwość zarejestrowania się jako administrator poprzez analizę kodu JS i uzyskania danych o kierowcach

16) Aplikacja elektronicznych rejestracji samochodowych w USA:
    - ta sama podatność co w F1
    - możliwość ustawienia statusu dowolnego samochodu jako kradziony

17) GoAnywhere  - aplikacja do wymiany plików:
    - poprzez specjalne wywołanie błędu 404 możba było wykonać dowolny kod na serwerze

18) Czym jest SSRF?

19) Oracle E-Business Suite:
    - z pomocą SSRF znaleziono podatność pozwalającą na wykonanie złośliwego oprogramowania na serwerze

20) Oracle Identity Manager oraz produkty firmy Ivanti:
    - możliwość RCE na serwerze
   
21) Urządzenie Ubiquiti:
    - w centralnym gateway można było odwołać się do specyficznego portu i wykonać skrypt na serwerze

22) Kamera PTZOptics:
    - błąd w oprogramowaniu i możliwość nieautoryzowanego zarządzania nią

23) FortiWeb -  zapora aplikacji internetowych:
    - SQL Injection na panelu logowania

24) CentOs - środowisko serwerowe:
    - możliwość zmiany uprawnień do plików bez autoryzacji

25) Omówienie OWASP Top 10 - raportu, który opisuje dziesięć najbardziej krytycznych zagrożeń dla bezpieczeństwa aplikacji internetowych:
    - najczęstsze podatności to błędy związane z uwierzytelnieniem, autoryzacją, kontrolą dostępu
    - najlepszy sposób ochrony to śledzenie najczęstszych ataków

