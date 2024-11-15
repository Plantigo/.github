# Plantigo - Inteligentny System Zarządzania Urządzeniami IoT

**Plantigo** to system zarządzania urządzeniami IoT, stworzony w celu monitorowania i optymalizacji procesów związanych z inteligentnymi urządzeniami. System łączy moduły nasłuchu danych, przetwarzania telemetrycznego oraz zarządzania urządzeniami, zapewniając kompleksową kontrolę nad ekosystemem IoT.

---

## Jak działa Plantigo?

1. **Nasłuchiwanie danych z urządzeń IoT:**
   - Moduł **IoT Listener** subskrybuje tematy MQTT i odbiera dane telemetryczne od podłączonych urządzeń.
   - Otrzymane dane są walidowane i zapisywane w bazie danych MongoDB.

2. **Przetwarzanie danych telemetrycznych:**
   - Moduł **Telemetry** pobiera dane z bazy MongoDB, przetwarza je (np. konwertuje jednostki, analizuje zmiany w czasie, wykrywa anomalie) i udostępnia przetworzone wyniki innym modułom.

3. **Zarządzanie urządzeniami:**
   - Moduł **Devices** komunikuje się z przetworzonymi danymi telemetrycznymi, aby sterować urządzeniami, konfigurować ich ustawienia oraz raportować stan systemu użytkownikom.

4. **Integracja z aplikacją mobilną i webową:**
   - System zapewnia dostęp do danych i konfiguracji urządzeń za pomocą aplikacji mobilnej oraz panelu administracyjnego w przeglądarce.

---

## Kluczowe funkcjonalności

- **Monitorowanie w czasie rzeczywistym:** Dane z urządzeń są odbierane i przetwarzane na bieżąco.
- **Zaawansowana analiza danych:** Moduł telemetry przetwarza dane i generuje przydatne informacje, takie jak wykrywanie awarii czy prognozy.
- **Zarządzanie urządzeniami:** Możliwość dodawania nowych urządzeń, aktualizacji ich ustawień oraz przeglądania historii działania.
- **Wysoka skalowalność:** System został zaprojektowany z myślą o obsłudze dużej liczby urządzeń IoT.

---
