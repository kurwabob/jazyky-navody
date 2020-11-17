# Nastavení produktů pro vazbu na aplikaci a studovnu

Tento návod popisuje systém tvorby SKU a nastavení objednávkové stránky u produktů.

## Popis

Pro správné fungování nákupu produktů z aplikace a studovny jsou nutné dvě věci:

1. správné nastavení SKU u produktu
2. přidání uživatelského pole s URL objednávkové stránky

## SKU

SKU produktu se skládá ze dvou částí – ID z Ruby a počtu měsíců předplataného nebo znak `a` pro jednorázový nákup.

Tvar SKU: `id-měsíce` nebo `id-a` pro jednorázový nákup. Znak `-` je krátká pomlčka / znak mínus. Nepoužívejte dlouhý spojovník apod!

Znamená to tedy že vždy bude více produktů se stejnou první částí SKU, které se budu lišit jen počtem měsíců předplatného ve druhé části za pomlčkou.

### Příklady

ID = 100, předplatné na 6 měsíců: `100-6`
ID = 100, předplatné na 1 měsíc: `100-1`
ID = 100, jednorázový nákup: `100-a`
