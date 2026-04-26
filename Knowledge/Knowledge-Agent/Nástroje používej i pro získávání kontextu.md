# Nástroje používej i pro získávání kontextu

## Trigger
- Agent potřebuje externí kontext
- MCP nebo konektor k datům
- read-only přístup ke službám

## Core rule
- Pokud agent potřebuje stejný externí kontext opakovaně → přidej řízený read-only konektor nebo rozcestník

## Decision rules
- Pokud agent opakovaně žádá stejný externí kontext → přidej řízený konektor nebo rozcestník
- Pokud nástroj slouží jen hypoteticky → nepřidávej ho do aktivního kontextu
- Pokud služba obsahuje citlivá data → začni read-only přístupem
- Kontextové nástroje snižují ruční kopírování informací
- Každý připojený nástroj zvyšuje oprávnění, údržbu a i tokenovou režii
- Přístup k datům musí být omezený podle rizika úkolu

## Use for
- napojení agenta na GitHub nebo issue tracker
- práci s firemní wiki
- hledání brand podkladů ve Figmě
- dotazování výzkumného notebooku

## Avoid
- Dávat agentovi široké zápisové přístupy jen proto, aby si mohl přečíst kontext

