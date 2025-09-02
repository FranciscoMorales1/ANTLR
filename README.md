FRANCISCO JOSE MORALES PULIDO


# Proyecto Calculadoras con ANTLR

## Proceso General de Creación

1. **Preparar herramientas**: Descargar ANTLR tool (antlr-4.13.2-complete.jar)
2. **Definir gramática**: Crear archivo .g4 con reglas léxicas y sintácticas
3. **Generar código**: Usar ANTLR tool para crear parsers/lexers en Java o Python
4. **Implementar visitor**: Crear clases que procesen el árbol sintáctico
5. **Compilar/ejecutar**: Compilar (Java) o ejecutar directamente (Python)

## Estructura de Carpetas
Cada calculadora tiene:
- `tool/` → JAR de ANTLR
- `grammar/` → Archivo .g4
- `src/` → Código principal y visitor
- `out/` o `gen/` → Código generado por ANTLR

## Ejecución

### Calculadoras Java:
```bash
java -cp "out;tool\antlr-4.13.2-complete.jar" Main
```

### Calculadora Python:
```bash
python -m src.main
```

## Modo de Uso
1. Escribir expresión (ej: `2 + 3 * 4;`)
2. Presionar Enter para nueva expresión
3. Al finalizar: Enter + CONTROL + Z + Enter (Windows)

Las calculadoras aceptan múltiples expresiones en una sola ejecución. Cada expresión debe terminar con salto de linea
