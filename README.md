## 🧩 Ejercicio 2: Creación de un recurso Patient (simulación)

### 🎯 Objetivo
Aprender a **crear y validar** un recurso FHIR tipo **Patient** en formato JSON.

### 📌 Instrucciones

1. Diseña un recurso **Patient** en formato **JSON**, utiliza tus datos personales para identificar la actividad elaborada:

```json
{
  "resourceType": "Patient",
  "id": "patient-example-1",
  "identifier": [
    {
      "use": "official",
      "type": {
        "coding": [
          {
            "system": "http://terminology.hl7.org/CodeSystem/v2-0203",
            "code": "NI",
            "display": "National unique individual identifier"
          }
        ]
      },
      "system": "http://example.org/dni",
      "value": "87654321"
    }
  ],
  "name": [
    {
      "use": "official",
      "family": "López",
      "given": ["María"]
    }
  ],
  "gender": "female",
  "birthDate": "1990-03-25"
}
```

2.  Validación del recurso

    Accede al validador online de FHIR:  
👉 [FHIR Validator](https://validator.fhir.org/)

3. Copia y pega el JSON en el validador para comprobar que cumple con la especificación. En caso que no cumple y se presente un error deberá corregirlo, tener en cuenta que cuando el JSON se encuentra OK ya no le saldrá ninguna alerta o observación.

### ✅ Resultado esperado

Si aparece el mensaje "Validation successful", significa que tu recurso es válido y está correctamente estructurado.

## 📤 Entrega de la tarea

Para completar esta actividad, debes enviar:

1. Un archivo **`patient.json`** con el recurso creado.  
2. Una **captura de pantalla** del validador FHIR mostrando el mensaje de **validación exitosa**.
