# Garmin Connect – automatische koppeling

De mobiele PWA kan TCX/GPX rechtstreeks importeren zonder server.

Voor automatische synchronisatie is de officiële Garmin Connect Developer Program-integratie nodig:

1. Vraag zakelijke toegang aan tot het Garmin Connect Developer Program.
2. Activeer minstens de Activity API. Optioneel: Training API om workouts/plannen naar Garmin Connect te sturen.
3. Registreer een OAuth 2.0 applicatie en callback-URL in het Garmin Developer Portal.
4. Bewaar client-id/client-secret uitsluitend server-side (niet in index.html/localStorage).
5. Implementeer server-endpoints, bijvoorbeeld:
   - GET /api/garmin/status
   - GET /api/garmin/connect (start OAuth)
   - GET /api/garmin/callback (OAuth callback)
   - POST /api/garmin/webhook (push/ping ontvangst volgens de goedgekeurde Garmin-documentatie)
   - GET /api/garmin/activities (genormaliseerde activiteiten voor de PWA)
6. Laat de server Garmin-activiteiten normaliseren naar: datum, sport, afstand_km, duur_min, gemiddelde_hartslag, optioneel tempo/cadans/hoogtemeters.

Belangrijk: concrete Garmin API-URL's, scopes en webhook-payloads worden pas ingevuld uit de documentatie die beschikbaar komt in het Developer Portal na goedkeuring. Gebruik geen onofficiële Garmin Connect-login/scraping voor productie.
