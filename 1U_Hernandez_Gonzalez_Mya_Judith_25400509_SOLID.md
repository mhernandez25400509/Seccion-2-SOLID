# 1. Principios SOLID

Los principios SOLID son un conjunto de cinco principios de diseño orientado a objetos que ayudan a crear software más mantenible, escalable y fácil de entender. Fueron propuestos por Robert C. Martin y son ampliamente usados en la ingeniería de software.

## 1.1 S – Single Responsibility Principle (SRP)

**Definición:**  
Una clase debe tener una sola razón para cambiar, es decir, debe encargarse de una única responsabilidad dentro del sistema.

**Ejemplo:**  
Una clase `Factura` que calcula el total y además imprime la factura viola el SRP.

Lo correcto sería:
- Una clase que calcule la factura.
- Otra clase que se encargue de imprimirla.

**¿Por qué es importante?**  
Porque facilita el mantenimiento del código. Si una clase tiene muchas responsabilidades, cualquier cambio puede provocar errores inesperados. Al tener una sola responsabilidad, el código es más claro, reutilizable y fácil de modificar.

---

## 1.2 O – Open/Closed Principle (OCP)

**Definición:**  
Las clases deben estar abiertas para extensión, pero cerradas para modificación.

**¿Por qué es importante?**  
Permite agregar nuevas funcionalidades sin alterar el código existente, reduciendo el riesgo de errores. Esto hace que el software sea más estable y fácil de escalar conforme crece el sistema.

---

## 1.3 L – Liskov Substitution Principle (LSP)

**Definición:**  
Los objetos de una clase base deben poder ser reemplazados por objetos de sus clases derivadas sin afectar el funcionamiento correcto del programa.

**¿Por qué es importante?**  
Garantiza que la herencia se utilice correctamente. Si una subclase no puede comportarse como su clase padre, el diseño es incorrecto y puede generar fallos lógicos en el sistema.

---

## 1.4 I – Interface Segregation Principle (ISP)

**Definición:**  
Los clientes no deben verse obligados a depender de interfaces que no utilizan.

**¿Por qué es importante?**  
Evita interfaces grandes y poco específicas. Al usar interfaces más pequeñas y enfocadas, el código se vuelve más flexible, comprensible y fácil de mantener.

---

## 1.5 D – Dependency Inversion Principle (DIP)

**Definición:**  
Los módulos de alto nivel no deben depender de módulos de bajo nivel. Ambos deben depender de abstracciones, no de implementaciones concretas.

**¿Por qué es importante?**  
Reduce el acoplamiento entre componentes del sistema. Esto facilita cambios, pruebas y reutilización del código, además de mejorar la arquitectura general del software.
