# Strings de búsqueda — Lens.org

**Fecha:** 5 de junio de 2026 | **Plataforma:** lens.org/lens/search/scholar

## S1 — Amplio (N=3.571 bruto)
```
("autism spectrum disorder" OR "ASD" OR "autism")
AND
("giftedness" OR "gifted" OR "high ability" OR "high abilities"
 OR "twice exceptional" OR "dual exceptionality" OR "intellectually gifted")
```

## S2 — Adultos Profesionales (N=999)
```
("autism spectrum disorder" OR "ASD" OR "autistic")
AND ("giftedness" OR "high ability" OR "twice exceptional" OR "high intellectual potential")
AND ("researcher" OR "scientist" OR "academic" OR "university"
     OR "higher education" OR "STEM" OR "professor")
```

## S3 — Diagnóstico Tardío y Enmascaramiento (N=450)
```
("autism spectrum disorder" OR "ASD")
AND ("giftedness" OR "high ability" OR "intellectually gifted")
AND ("late diagnosis" OR "late identified" OR "masking"
     OR "camouflaging" OR "compensation" OR "adult diagnosis")
```

## S4 — Neurodiversidad en Entornos Laborales (N=120)
```
("autistic" OR "autism spectrum") AND ("neurodiversity" OR "neurodivergent")
AND ("academic career" OR "research career" OR "workplace" OR "employment"
     OR "scientists" OR "professionals")
AND ("high ability" OR "gifted" OR "twice exceptional")
```

## S5 — Español / Latinoamérica (N=360)
```
("trastorno del espectro autista" OR "TEA" OR "autismo")
AND ("altas capacidades" OR "superdotación" OR "doble excepcionalidad"
     OR "alta capacidad intelectual")
AND ("investigación" OR "academia" OR "universidad" OR "investigadores")
```

## Notas
- S1-amplio y S1-base: archivos idénticos (MD5 confirmado). Usar S1-amplio.
- S3 completamente contenido en S1 (solapamiento 100%).
- S5 con S1: solapamiento 5% — corpus iberoamericano casi independiente.
