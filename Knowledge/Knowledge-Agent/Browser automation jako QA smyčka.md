# Browser automation jako QA smyčka

## Trigger
- frontend QA
- lokální webová aplikace
- ověření uživatelského toku

## Core rule
- Pokud UI workflow závisí na klikání, formulářích nebo navigaci → ověř ho v reálném browseru

## Decision rules
- Pokud workflow závisí na klikání, formulářích nebo navigaci → spusť browser QA
- Pokud agent najde chybu v UI toku → oprav kód a zopakuj průchod
- Pokud potřebuješ audit viditelného stavu → ukládej screenshoty
- Reálný browser odhalí chyby, které statická kontrola mine
- Screenshoty zvyšují auditovatelnost UI testu
- Test-oprava-test smyčka snižuje riziko regresí v toku

## Use for
- formulářích po krocích
- e2e kontrole webové aplikace
- testování onboarding flow
- ověření lokálního frontend serveru

## Avoid
- Považovat hotový kód za ověřený bez průchodu v reálném browseru

