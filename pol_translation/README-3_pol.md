# linea-contracts

## Audyty
### Czwarta runda audytów (Najnowsza)

**Open Zeppelin**
- Audyt optymalizacji gazu: https://blog.openzeppelin.com/linea-gas-optimizations-audit

**Cyfrin**
- Pełny audyt kodu źródłowego, w tym optymalizacje gazu i aktualizacje TokenBridge: https://github.com/Cyfrin/cyfrin-audit-reports/blob/main/reports/2024-05-24-cyfrin-linea-v2.0.pdf 

### Trzecia runda audytów
**Open Zeppelin**

- Audyt składania blobów: https://blog.openzeppelin.com/linea-blob-submission-audit

### Druga runda audytów

**Diligence**
- Audyt agregacji dowodów, kompresji danych i aktualizacji usługi wiadomości: https://consensys.io/diligence/audits/2024/01/linea-contracts-update/

**Open Zeppelin**

- Audyt agregacji dowodów, kompresji danych i aktualizacji usługi wiadomości: https://blog.openzeppelin.com/linea-v2-audit

### Pierwsza runda audytów

**Diligence**

- Plonk Verifier: https://consensys.io/diligence/audits/2023/06/linea-plonk-verifier/
- Usługa wiadomości i Rollup https://consensys.io/diligence/audits/2023/06/linea-message-service/
- Canonical Token Bridge: https://consensys.io/diligence/audits/2023/06/linea-canonical-token-bridge/

**Open Zeppelin**

- Audyt mostu Linea: https://blog.openzeppelin.com/linea-bridge-audit-1
- Audyt Verifier Linea: https://blog.openzeppelin.com/linea-verifier-audit-1



---

## Instalacja i testowanie

Aby uruchomić testy rozwiązania, raportowanie pokrycia i zużycia gazu, upewnij się, że masz zainstalowany pnpm, a następnie
```
# Install all the dependencies

pnpm install

pnpm run test

pnpm run test:reportgas

pnpm run coverage
```