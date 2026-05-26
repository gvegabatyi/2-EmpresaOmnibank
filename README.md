# OmniBank Fintech & Ciberseguridad - Portafolio de Cumplimiento
> **Expediente de Auditoria Legal y Tecnica bajo la Ley 21.719 (Proteccion de Datos Personales) y Ley 21.663 (Ley Marco de Ciberseguridad) en Chile.**

---

##  Descripcion del Proyecto
Este repositorio contiene el **Expediente de Cumplimiento Normativo y Gestion de Riesgos** de **OmniBank**, la filial financiera y fintech de **Holding OmniGroup**. 

A diferencia de otras filiales, OmniBank opera bajo un estándar de **especialidad normativa extrema** debido a su naturaleza y a que ha sido precalificado como **Operador de Importancia Vital (OIV)** por la Agencia Nacional de Ciberseguridad (ANCI). Esto clasifica sus sistemas y base de datos como **Infraestructura Critica de la Informacion (ICI)** de interes nacional.

---

## Contenido del Portafolio (Expedientes y Entregables)

El portafolio esta estructurado sistematicamente en **5 fases clave**, representadas en los documentos maestros PDF incluidos en este repositorio:

| # | Archivo PDF / Documento | Descripcion del Entregable | Marco Legal Aplicable |
| :--- | :--- | :--- | :--- |
| 📄 | [**01_OMNIBANK_AUDITORIA_FASE1.pdf**](./01_OMNIBANK_AUDITORIA_FASE1.pdf) | **Contexto, Licitud y Clasificacion**: Diagnostico del activo critico `omnibank_clientes.csv` y gap analysis inicial. | Ley N° 21.719 / Ley N° 21.663 / Art. 154 LGB |
| 📄 | [**02_OMNIBANK_RIESGOS_ISO31000.pdf**](./02_OMNIBANK_RIESGOS_ISO31000.pdf) | **Matriz de Riesgo ISO 31000**: Evaluacion sistematica de amenazas financieras, operacionales y reputacionales. | Norma ISO 31000 / ISO 27001 |
| 📄 | [**03_OMNIBANK_TRATAMIENTO_RIESGO.pdf**](./03_OMNIBANK_TRATAMIENTO_RIESGO.pdf) | **Plan de Tratamiento y Mitigacion**: Medidas de control tecnico (red team, segmentacion) y legal (contratos de transmision). | Ley N° 21.663 / Controles CIS / ISO 27701 |
| 📄 | [**04_OmniBank_Conclusion_y_Proyeccion.pdf**](./04_OmniBank_Conclusion_y_Proyeccion.pdf) | **Gobernanza y Conclusiones del DPO**: Estrategia de segregacion de funciones, organigrama de control y accountability. | Principio de Responsabilidad Proactiva |
| 📄 | [**05_OmniBank_Reporte_Tecnico.pdf**](./05_OmniBank_Reporte_Tecnico.pdf) | **Informe de Ingenieria Forense y Criptografia**: Propuesta de blindaje para el dataset critico y controles de acceso restringido. | Ley N° 21.663 / Criptografia Simetrica AES-256 |

---

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
* Implementacion de un **Manual del Delegado de Proteccion de Datos (DPD)** y canales ARCO específicos.

---

## Descargo de Responsabilidad / Disclaimer (Dataset)
El archivo de datos **`omnibank_clientes.csv`** que forma parte de este portafolio de evidencias es un **dataset 100% ficticio, simulado y sintetizado** con fines estrictamente pedagogicos, academicos y de evaluacion de compliance. 

*   **No contiene ni representa informacion real** de ningun cliente, transaccion, cuenta bancaria ni entidad financiera real.
*   Toda relacion de variables, saldos o scores ha sido generada artificialmente para evaluar la madurez de los sistemas de gestion de riesgos y el cumplimiento normativo (Leyes 21.719 y 21.663).
*   Cualquier coincidencia con personas, datos o situaciones reales es una absoluta coincidencia.

---

## Responsable de la Auditoria
**Gonzalo Vega Batyi**  
*Abogado Experto en Ciberseguridad, Proteccion de Datos y DPO (Delegado de Proteccion de Datos).*  
🔗 [LinkedIn Profile](https://www.linkedin.com/in/gvegabatyi)  
*Holding OmniGroup: Compliance & Risk Lab*
