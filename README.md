##  Descripcion del Proyecto
Este repositorio contiene el **Expediente de Cumplimiento Normativo y Gestion de Riesgos** de **OmniBank**, la filial financiera y fintech de **Holding OmniGroup**. 

A diferencia de otras filiales, OmniBank opera bajo un estándar de **especialidad normativa extrema** debido a su naturaleza y a que ha sido precalificado como **Operador de Importancia Vital (OIV)** . Esto clasifica sus sistemas y base de datos como **Infraestructura Critica de la Informacion (ICI)** de interes nacional.

> **Nota de Cumplimiento GRC:** Dada la naturaleza de este módulo como simulación de infraestructura crítica financiera, se ha elevado el estándar de seguridad a nivel de **Operador de Importancia Vital (OIV)**. 
> 
> A diferencia de otros laboratorios de la holding, en **OmniBank** se aplican controles de inmutabilidad técnica para garantizar que la evidencia no pueda ser alterada, asegurando la cadena de custodia desde el diseño (Privacy by Design).


## Control de Integridad Documental (SHA-256)

Para garantizar el **No Repudio** y la inmutabilidad de los hallazgos de auditoría, se adjunta la firma digital (Hash) de cada activo crítico. Cualquier alteración bit a bit del archivo invalidará su correspondencia con esta tabla.

| Recurso Documental | Función GRC | Huella Digital (SHA-256 Hash) |
| :--- | :--- | :--- |
| **01_OMNIBANK_AUDITORIA_FASE1.pdf** | Informe de Auditoría Inicial | `C44FA3DBF96EBB08B62B9625C21831218708925F5CF7A6AD978CA9464299153F` |
| **02_OMNIBANK_RIESGOS_ISO31000.pdf**| Matriz de Riesgos ISO 31000 | `A48D050403905462FD212899B6C418867B371422A1803F3C7B730DB7D939E0B9` |
| **03_OMNIBANK_TRATAMIENTO_RIESGO.pdf** | Plan de Tratamiento de Riesgos | `5AEC8BE5790BA458D28B4877951C8ADF5EAD952BFAA7229CD7388EFB329FC894` |
| **04_OmniBank_Conclusion_y_Proyeccion.pdf** | Dictamen de Cierre y Proyección | `DC005C17D85573CAAF608D83F1
# OmniBank Fintech & Ciberseguridad - Portafolio de Cumplimiento
> **Expediente de Auditoria Legal y Tecnica bajo la Ley 21.719 (Proteccion de Datos Personales) y Ley 21.663 (Ley Marco de Ciberseguridad) en Chile.**


## Hallazgos Criticos Detectados (Gap Analysis)
Durante la auditoria legal-tecnica se identificaron las siguientes brechas de alto impacto:
1. **Quebre del Principio de Finalidad (Art. 9 Ley 21.719):** Flujo no autorizado de datos financieros y de perfilamiento crediticio (`Score_DICOM`, `Saldo_Promedio`) desde OmniBank hacia la filial de Retail con fines de marketing.
2. **Vulnerabilidad de Infraestructura Critica (Ley 21.663):** Ausencia de segmentacion de red y "Air Gapping" entre el entorno del Retail y el Core Bancario, permitiendo un vector de ataque transfronterizo.
3. **Falta de Custodia y Secreto Bancario (Art. 154 LGB):** Acceso libre de lectura del personal corporativo de TI al dataset de clientes sin protocolos de autorizacion ni cifrado.

---

## Controles de Mitigacion Propuestos
* **Cifrado AES-256** del dataset financiero `omnibank_clientes.csv`.
* **Air Gapping** fisico y logico en redes financieras.
* Modificacion al **Reglamento Interno (RIHS)** del Holding para tipificar sanciones severas por filtracion de datos de infraestructura critica.
* Implementacion de un **Manual del Delegado de Proteccion de Datos (DPD)** y canales ARSOBP específicos.

---

## Descargo de Responsabilidad / Disclaimer (Dataset)
El archivo de datos **`omnibank_clientes.csv`** que forma parte de este portafolio de evidencias es un **dataset 100% ficticio, simulado y sintetizado** con fines estrictamente pedagogicos, academicos y de evaluacion de compliance. 

*   **No contiene ni representa informacion real** de ningun cliente, transaccion, cuenta bancaria ni entidad financiera real.
*   Toda relacion de variables, saldos o scores ha sido generada artificialmente para evaluar la madurez de los sistemas de gestion de riesgos y el cumplimiento normativo (Leyes 21.719 y 21.663).
*   Cualquier coincidencia con personas, datos o situaciones reales es una absoluta coincidencia.

---

## Responsable de la Auditoria
**Gonzalo Vega Batyi**  
*Abogado GRC Ciberseguridad, Proteccion de Datos.*  
🔗 [LinkedIn Profile](https://www.linkedin.com/in/gvegabatyi)  
*Holding OmniGroup: Compliance & Risk Lab*
