<!-- ELUCENIA technical documentation · padua · es · no clinical/professional/rights approval -->

# Puntuación de Padua

[condiciones, fuentes y permisos](https://elucenia.org/es/herramientas/padua)

## Cómo usar

Utilice la herramienta en el portal o abra index.html mediante un servidor HTTP local. Seleccione el idioma, complete los campos y calcule.

## Entradas y unidades

### Cáncer activo (metástasis o quimioterapia/radioterapia en los últimos 6 meses)

`cancer`

### TEV previa (excepto trombosis venosa superficial)

`tev`

### Movilidad reducida (reposo en cama, con permiso para ir al baño, durante ≥ 3 días)

`mobilidade`

### Trombofilia conocida

`trombofilia`

### Traumatismo o cirugía en el último mes

`trauma`

### Edad ≥ 70 años

`idade`

### Insuficiencia cardíaca y/o respiratoria

`icc`

### Infarto agudo de miocardio o ictus isquémico

`iam`

### Infección aguda y/o enfermedad reumatológica

`infeccao`

### Obesidad (IMC ≥ 30 kg/m²)

`obesidade`

### Tratamiento hormonal en curso

`hormonio`

## Edición del método

Padua Prediction Score/Barbar 2010: 11 factores, 0–20; paciente médico hospitalizado

## Fórmula documentada

3 puntos: cáncer activo, TEV previo, movilidad reducida, trombofilia · 2 puntos: traumatismo o cirugía reciente · 1 punto: edad ≥ 70, insuficiencia cardíaca/respiratoria, IAM o ictus isquémico, infección aguda o enfermedad reumatológica, obesidad, terapia hormonal. Máximo: 20.

## Límites y población

El Padua se estudió en pacientes médicos ingresados en medicina interna, con seguimiento del tromboembolismo sintomático hasta 90 días. La estratificación trombótica debe acompañarse de evaluación del sangrado, las contraindicaciones y el protocolo de profilaxis. El total no sustituye este análisis ni implica su aplicación automática a la población quirúrgica.

## Referencias

- [Barbar S et al. A risk assessment model for the identification of hospitalized medical patients at risk for venous thromboembolism: the Padua Prediction Score. J Thromb Haemost, 2010.](https://doi.org/10.1111/j.1538-7836.2010.04044.x)

- [Kahn SR et al. Prevention of VTE in nonsurgical patients: antithrombotic therapy and prevention of thrombosis, 9th ed: American College of Chest Physicians evidence-based clinical practice guidelines. Chest, 2012.](https://doi.org/10.1378/chest.11-2296)

## Reproducir las pruebas técnicas

Ejecute node test.cjs en el directorio raíz de este repositorio para repetir los casos sintéticos registrados. Se conservan las entradas, los resultados esperados y las tolerancias originales. Las pruebas técnicas no constituyen validación clínica.

```sh
node test.cjs
```

tool.json contiene las fuentes, la edición y el alcance de la revisión. examples.json conserva las entradas y los resultados esperados de los casos sintéticos; results.json registra los resultados obtenidos.

[Ficha y referencias](../tool.json) · [Código JavaScript](../calculator.js) · [Casos de referencia](../examples.json) · [results.json](../results.json)

## Revisión y condiciones de uso

No se ha realizado una revisión clínica independiente.

Esta interfaz es una traducción de elaboración propia, no una edición oficial o certificada. No se han realizado la revisión clínica independiente, la revisión lingüística profesional ni la autorización de derechos de los instrumentos.

Resultado de la fórmula o clasificación. La interpretación, la conducta y la aplicabilidad dependen de la evaluación profesional y de la fuente seleccionada.

## Licencia y atribución

Apache-2.0 se aplica únicamente al código de ELUCENIA. Los derechos de los instrumentos, publicaciones, traducciones y datos permanecen en manos de sus respectivos titulares. Conserve LICENSE y NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026
