# 🛠️ Taller 6: Checklist de Cumplimiento Normativo  
### Curso: Arquitectura Empresarial – Universidad de La Sabana  
**Estudiante:** Valentina Rodriguez Romero
**Profesor:** César Augusto Vega Fernández  
**Fecha:** 1 de noviembre de 2025  

---

## 🎯 Objetivo
Verificar el cumplimiento de aspectos **legales, normativos y de protección de datos** aplicables a los sistemas del caso base **GobData** y del cliente real **Compulens**, utilizando un checklist alineado con los marcos:

- **Ley 1581 de 2012** y **Decreto 1377 de 2013** – Protección de Datos Personales (Colombia)  
- **ISO/IEC 27001:2022** – Seguridad de la Información  
- **GDPR (UE 2016/679)** – Reglamento General de Protección de Datos  
- **Guía SIC – Habeas Data y Datos Sensibles**

El taller busca fortalecer la capacidad de **evaluar el cumplimiento normativo** dentro de la arquitectura empresarial, garantizando la confianza, trazabilidad y seguridad de los sistemas analizados.

---

## 🧱 Estructura del repositorio

```
taller-06-normatividad/
├── README.md 
├── clase/
│ ├── checklist-gobdata.xlsx 
│ └── notas.md 
└── entrega/
├── checklist-cliente.xlsx 
├── informe.md 
└── referencias.md 
```

---

## 🧩 Parte 1 – Caso base: **GobData**

- Se aplicó el checklist de cumplimiento a un **portal estatal de trámites ciudadanos**.  
- Se evaluaron controles de **consentimiento informado, seguridad de la información, trazabilidad, retención y roles de acceso**.  
- Principales hallazgos:
  - Falta de política de retención documental.
  - Cifrado incompleto en reposo.
  - Ausencia de evaluaciones de impacto (DPIA).
- Se propusieron **acciones correctivas** de corto plazo: política de retención, cifrado uniforme, y DPIA para módulos sensibles.

📂 Archivos:  
`clase/checklist-gobdata.xlsx`  
`clase/notas.md`

---

## 🧠 Parte 2 – Cliente real: **Compulens**

- Se aplicó el mismo checklist al sistema de **toma de pedidos y gestión ERP** de Compulens S.A.S.  
- Se analizaron los flujos de información actuales y la arquitectura **TO-BE** propuesta (con chatbot OCR, integración ERP y autenticación reforzada).  
- Se evaluó el cumplimiento con las normativas nacionales y la **ISO 27001**.

**Nivel de cumplimiento estimado:**  
| Categoría | % Cumplimiento |
|------------|----------------|
| Gobernanza legal | 70% |
| Consentimiento | 80% |
| Seguridad | 75% |
| Retención | 70% |
| Privacidad por diseño | 60% |
| Derechos del titular | 65% |

**Promedio general:** 70% – *Cumplimiento medio-alto.*

📌 **Principales brechas:**  
- Contratos con terceros sin cláusulas de seguridad.  
- Consentimiento no diferenciado para imágenes biométricas.  
- Falta de portal para derechos ARCO.  
- No hay sistema central de monitoreo (SIEM).  
- DPIA no aplicado a módulos OCR/chatbot.  

**Recomendaciones clave:**  
1. Actualizar contratos de tratamiento de datos con terceros.  
2. Implementar SIEM y rotación de llaves KMS.  
3. Realizar DPIA en nuevos módulos de automatización.  
4. Implementar portal digital para derechos ARCO.  

📂 Archivos:  
`entrega/checklist-cliente.xlsx`  
`entrega/informe.md`  
`entrega/referencias.md`

---

## 📚 Referencias legales y técnicas

- Ley 1581 de 2012 – Protección de Datos Personales  
- Decreto 1377 de 2013 – Reglamentación de la Ley 1581  
- ISO/IEC 27001:2022 – Gestión de la seguridad de la información  
- GDPR (UE 2016/679) – Reglamento General de Protección de Datos  
- Guía SIC – Tratamiento de datos personales sensibles  
- Resolución 1995 de 1999 – Historias clínicas (MinSalud)  
- Circular MinTIC 01 de 2021 – Lineamientos de seguridad digital  


---

## ✅ Licencia
Uso académico bajo licencia **MIT** – Curso de Arquitectura Empresarial, Universidad de La Sabana.
