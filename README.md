# Procesado en MeshLab: The Map of the World Tablet

Repositorio para la práctica de procesado y optimización de mallas 3D.

### Resumen de Datos
* Entrada: Nube de puntos PLY (1,651,862 vértices) con color por vértice.
* Salida: Malla optimizada 10K - verts en formato X3D.
* Reducción: 99.39% de la carga poligonal.

### Flujo de trabajo de Limpieza y Optimización
1. Reconstrucción: Generación de superficie mediante Screened Poisson.
2. Reparación Topológica:
   * Eliminación de 37,916 T-vertices.
   * Fusión de 116,625 vértices (Merge Close Vertices).
   * Limpieza de caras auto-intersectantes y cierre de huecos.
3. Simplificación: Reducción a 10,000 vértices mediante Quadric Edge Collapse Decimation preservando la estanqueidad (manifold) de la malla.
4. Texturizado: Generación de Voronoi Atlas y transferencia de color de vértice a textura de imagen.

---
Esta práctica forma parte del Tema 5: Publicación y Difusión, incluido en el Módulo 2: Digitalización del Patrimonio Cultural; perteneciente al curso de la UNED "Tecnologías Avanzadas para la Gestión y Documentación del Patrimonio Cultural", en su edición de 2025.
