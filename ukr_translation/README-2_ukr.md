# linea-contracts

## Аудити
### Четвертий раунд аудиту (останній)

**Open Zeppelin**
- Аудит оптимізації газу: https://blog.openzeppelin.com/linea-gas-optimizations-audit

**Cyfrin**
- Аудит усієї кодової бази, включаючи оптимізації газу та оновлення TokenBridge: https://github.com/Cyfrin/cyfrin-audit-reports/blob/main/reports/2024-05-24-cyfrin-linea-v2.0.pdf 

### Третій раунд аудиту
**Open Zeppelin**

- Аудит відправки Blob: https://blog.openzeppelin.com/linea-blob-submission-audit

### Другий раунд аудиту

**Diligence**
- Аудит оновлень агрегації доказів, стиснення даних і служби повідомлень:  https://consensys.io/diligence/audits/2024/01/linea-contracts-update/

**Open Zeppelin**

- Аудит оновлень агрегації доказів, стиснення даних і служби повідомлень:  https://blog.openzeppelin.com/linea-v2-audit

### Перший раунд аудиту

**Diligence**

- Plonk Verifier: https://consensys.io/diligence/audits/2023/06/linea-plonk-verifier/
- Служба повідомлень та Rollup: https://consensys.io/diligence/audits/2023/06/linea-message-service/
- Канонічний Token Bridge: https://consensys.io/diligence/audits/2023/06/linea-canonical-token-bridge/

**Open Zeppelin**

- Аудит мосту Linea: https://blog.openzeppelin.com/linea-bridge-audit-1
- Аудит верифікатора Linea: https://blog.openzeppelin.com/linea-verifier-audit-1



---

## Встановлення та тестування

Щоб запустити тести рішення, перевірку покриття та звіти про витрати газу, переконайтеся, що ви встановили pnpm, а потім
```
# Install all the dependencies

pnpm install

pnpm run test

pnpm run test:reportgas

pnpm run coverage
```