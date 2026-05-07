# Taller en Clase — POO en Python
## Figuras Geométricas

**Autor:** Elian Andrade  
**Fecha:** 06 de mayo de 2026  
**Hora:** 22:30  
**Lenguaje:** Python 3  

---

## Descripción

Programa que implementa los conceptos de **Programación Orientada a Objetos (POO)** en Python usando figuras geométricas como contexto práctico. Se aplican los pilares de encapsulamiento, herencia, sobrescritura de métodos y polimorfismo.

---

## Estructura de Clases

FigurasGeometricas (clase base)
├── Rectangulo
├── Triangulo
└── Elipse

---

## Conceptos Implementados

- **Encapsulamiento:** atributos privados con `__`, getters y setters con `@property` y validaciones
- **Herencia:** las subclases heredan de `FigurasGeometricas`
- **Sobrescritura:** cada subclase redefine `area()`, `perimetro()` y `__str__()`
- **Polimorfismo:** método `describir()` con comportamiento distinto por clase

---

## Fórmulas Utilizadas

| Figura | Área | Perímetro |
|---|---|---|
| Rectángulo | alto × ancho | 2 × (alto + ancho) |
| Triángulo | (base × altura) / 2 | a + b + hipotenusa (Pitágoras) |
| Elipse | π × a × b | Aproximación de Ramanujan |

---

## Evidencias de Ejecución

### 1. Figura base — getters y setters

[1] Figura base creada:
    alto  (getter) → 3 cm
    ancho (getter) → 7 cm

[2] Valores modificados con setters:
    alto  (setter) → 11 cm
    ancho (setter) → 20 cm
    Área base      → 220.00 cm²
    Perímetro base → 62.00 cm

### 2. Validación del setter

[3] Validación del setter (valor negativo):
     Error capturado correctamente: El alto debe ser un valor positivo.

### 3. Herencia y sobrescritura

Rectángulo  | Alto: 8 cm  | Ancho: 15 cm | Área: 120.00 cm² | Perímetro: 46.00 cm
Triángulo   | Alto: 6 cm  | Base: 5 cm   | Área: 15.00 cm²  | Perímetro: 18.81 cm
Elipse      | Semi-eje a: 10 cm | Semi-eje b: 4 cm | Área: 125.66 cm² | Perímetro: 47.10 cm

### 4. Setter desde subclase

[4] Cambiar dimensiones del rectángulo con setter:
Rectángulo  | Alto: 14 cm | Ancho: 9 cm  | Área: 126.00 cm² | Perímetro: 46.00 cm

### 5. Polimorfismo — método describir()

[1] Soy una figura geométrica genérica.
[2] Soy un Rectángulo de 8 cm de alto y 15 cm de ancho.
[3] Soy un Triángulo con altura 6 cm y base 5 cm.
[4] Soy una Elipse con semi-eje a=10 cm y semi-eje b=4 cm.

---

## Cómo ejecutar

python laura_y_jair.py

---

## Requisitos

- Python 3.10 o superior
- No requiere librerías externas (solo `math` de la librería estándar)
