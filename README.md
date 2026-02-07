# 🎨 Image Filter Pro

Editor de imágenes profesional con filtros preestablecidos de alta calidad, diseñado para fotógrafos y entusiastas de la edición fotográfica.

![Python Version](https://img.shields.io/badge/python-3.8+-blue.svg)
![License](https://img.shields.io/badge/license-GPLv3-blue.svg)

## ✨ Características

- 🖼️ **Múltiples formatos soportados**: JPG, PNG, WEBP, BMP, TIFF
- 🎭 **Filtros profesionales predefinidos**:
  - 🔍 **HD**: Mejora la nitidez y reduce el ruido
  - 📼 **Retro**: Estilo vintage con viñeta
  - 🌈 **Colores Vivos**: Ideal para paisajes
  - ⚫ **Blanco y Negro**: Conversión monocromática artística
  - 🟤 **Sepia**: Tono nostálgico
  - ❄️ **Cool**: Tonalidades frías
  - 🔥 **Warm**: Tonalidades cálidas
- 👁️ **Previsualización**: Ve el resultado antes de guardar
- 💾 **Exportación optimizada**: Salida en formato PNG de máxima calidad
- 🎯 **Interfaz CLI intuitiva**: Menús interactivos y coloridos

## 🚀 Instalación

### Requisitos previos
- Python 3.8 o superior
- pip

### Pasos

1. **Clonar el repositorio**
```bash
git clone https://github.com/DiegoFernandoChavarroCastillo/ImgEditor
cd ImgEditor
```

2. **Crear entorno virtual (recomendado)**
```bash
python -m venv venv

# En Windows
venv\Scripts\activate

# En Linux/Mac
source venv/bin/activate
```

3. **Instalar dependencias**
```bash
pip install -r requirements.txt
```

## 📖 Uso

### Modo interactivo (recomendado)
```bash
python -m src.main
```

### Modo comando directo (futuro)
```bash
python -m src.main --image foto.jpg --filter hd --output salida.png
```

## 🎮 Guía de Uso

1. **Ejecuta la aplicación**
2. **Selecciona tu imagen** desde el explorador de archivos
3. **Elige un filtro** del menú interactivo
4. **Previsualiza** el resultado
5. **Guarda** si te gusta o prueba otro filtro

## 🎨 Filtros Disponibles

| Filtro | Descripción | Mejor para |
|--------|-------------|------------|
| HD | Mejora nitidez y reduce ruido | Fotos desenfocadas |
| Retro | Efecto vintage con viñeta | Retratos, fotos urbanas |
| Colores Vivos | Aumenta saturación y contraste | Paisajes, naturaleza |
| Blanco y Negro | Conversión monocromática | Arte, retratos dramáticos |
| Sepia | Tono cálido nostálgico | Fotos antiguas, vintage |
| Cool | Tonalidades azuladas | Escenas nocturnas, invierno |
| Warm | Tonalidades naranjas | Atardeceres, escenas cálidas |

## 🛠️ Tecnologías

- **Python 3.8+**
- **Pillow**: Manipulación de imágenes
- **OpenCV**: Filtros avanzados
- **NumPy**: Operaciones matriciales
- **Rich**: Terminal moderna
- **Inquirer**: Menús interactivos

## 📂 Estructura del Proyecto
```
image-filter-pro/
├── src/
│   ├── filters/       # Todos los filtros
│   ├── core/          # Lógica principal
│   └── ui/            # Interfaz de usuario
├── tests/             # Tests unitarios
└── output/            # Imágenes procesadas
```

## 🗺️ Roadmap

### MVP (v0.1.0) ✅
- [x] Carga de imágenes en múltiples formatos
- [x] 7+ filtros predefinidos
- [x] Sistema de previsualización
- [x] Exportación optimizada
- [x] Interfaz CLI

### Futuras versiones

#### v0.2.0
- [ ] Más filtros (dramático, suave, vintage avanzado)
- [ ] Procesamiento por lotes
- [ ] Historial de ediciones

#### v0.3.0
- [ ] Ajustes manuales de parámetros
- [ ] Filtros personalizados guardables
- [ ] Comparación lado a lado

#### v1.0.0
- [ ] GUI con Tkinter/PyQt
- [ ] Plugin system para filtros custom
- [ ] Integración con redes sociales
- [ ] Exportación a múltiples formatos

## 🤝 Contribuir

¡Las contribuciones son bienvenidas! Por favor:

1. Fork el proyecto
2. Crea tu rama (`git checkout -b feature/AmazingFilter`)
3. Commit tus cambios (`git commit -m 'Add: Filtro increíble'`)
4. Push a la rama (`git push origin feature/AmazingFilter`)
5. Abre un Pull Request

## 📝 Ejemplos de código

### Añadir un nuevo filtro
```python
# src/filters/mi_filtro.py
from .base_filter import BaseFilter
import cv2

class MiFiltroCustom(BaseFilter):
    name = "Mi Filtro"
    description = "Descripción de mi filtro"
    
    def apply(self, image):
        # Tu lógica aquí
        processed = cv2.GaussianBlur(image, (15, 15), 0)
        return processed
```

## 📄 Licencia

Este proyecto está bajo la Licencia Pública General de GNU v3.0 (GPL v3).

![GNU GPL v3](https://www.gnu.org/graphics/gplv3-127x51.png)

Ver el archivo `LICENSE` para más detalles.

## 👤 Autor

**Tu Nombre**
- GitHub: [@DiegoFernandoChavarroCastillo](https://github.com/DiegoFernandoChavarroCastillo)

## 🙏 Agradecimientos

- Comunidad de OpenCV
- Equipo de Pillow
- Todos los contribuidores

---

⭐ Si este proyecto te fue útil, ¡dale una estrella en GitHub!