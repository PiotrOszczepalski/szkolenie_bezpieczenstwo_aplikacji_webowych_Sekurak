Szkolenie: "Dlaczego hackowanie aplikacji webowych jest proste? Przegląd najnowszych/najciekawszych luk bezpieczeństwa w aplikacjach"

Autor: Michał Sajdak, Sekurak

Spis treści:

1) Aplikacja AI do analizowania dokumentów i pomocy w wygrywaniu przetargów firmy Minerva:
   - bezpośrednio poprzez przeglądarkę można było dostać się do listy użytkowników oraz konwersacji z chatem AI
   - można było również uzyskać dostęp do poufnych dokumentów

2) Aplikacja FlowiseAi do tworzenia agentów AI:
   - podająć adres e-mail dowolnego użytkownika w funkcji resetu hasła można było zresetować mu hasło i dostać się na jego konto
  
3) Aplikacja AI dla prawników FileVine:
   - odwołanie w komunikacji http do zasobu na AWS, w odpowiedzi można było uzyskać uwierzytelnienie dla pełnego administratora
  
4) McDelivery w Indiach:
   - możliwość zmiany wartości koszyka i zamówienia jedzenia prawie za darmo
  
5) MC Hire:
   - poprzez login i hasło 123456 można było dostać się do panelu admistratora testowej restauracji McDonald's oraz uzyskać dostęp do rozmów kandydatów ubiegających się o pracę

6) Aplikacja Subaru:
   - łatwy reset hasła w ukrytym panelu logowania i dostęp do aplikacji, gdzie można było poznać lokalizację samochodów

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
