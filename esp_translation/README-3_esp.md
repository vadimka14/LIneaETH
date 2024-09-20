# contratos de Linea

## Auditorías
### Cuarta Ronda de Auditoría (Más Reciente)

**Open Zeppelin**
- Auditoría de optimización de gas: https://blog.openzeppelin.com/linea-gas-optimizations-audit

**Cyfrin**
- Auditoría completa del código, incluyendo optimizaciones de gas y actualizaciones de TokenBridge: https://github.com/Cyfrin/cyfrin-audit-reports/blob/main/reports/2024-05-24-cyfrin-linea-v2.0.pdf 

### Tercera Ronda de Auditoría
**Open Zeppelin**

- Auditoría de presentación de blobs: https://blog.openzeppelin.com/linea-blob-submission-audit

### Segunda Ronda de Auditoría

**Diligence**
- Auditoría de agregación de pruebas, compresión de datos y actualizaciones del servicio de mensajes: https://consensys.io/diligence/audits/2024/01/linea-contracts-update/

**Open Zeppelin**

- Auditoría de agregación de pruebas, compresión de datos y actualizaciones del servicio de mensajes: https://blog.openzeppelin.com/linea-v2-audit

### Primera Ronda de Auditoría

**Diligence**

- Verificador de Plonk: https://consensys.io/diligence/audits/2023/06/linea-plonk-verifier/
- Servicio de Mensajes y Rollup: https://consensys.io/diligence/audits/2023/06/linea-message-service/
- Canonical Token Bridge: https://consensys.io/diligence/audits/2023/06/linea-canonical-token-bridge/

**Open Zeppelin**

- Auditoría del Puente Linea: https://blog.openzeppelin.com/linea-bridge-audit-1
- Auditoría del Verificador Linea: https://blog.openzeppelin.com/linea-verifier-audit-1



---

## Instalación y pruebas

Para ejecutar las pruebas de la solución, cobertura e informes de gas, asegúrate de instalar pnpm y luego
```
# Install all the dependencies

pnpm install

pnpm run test

pnpm run test:reportgas

pnpm run coverage
```