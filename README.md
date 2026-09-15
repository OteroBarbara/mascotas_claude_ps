# Prompt utilizado: 

Actúa como un desarrollador web experto en accesibilidad (WCAG 2.1 / 2.2 y WAI-ARIA) y desarrollo frontend estático.

Necesito que generes un sitio web estático utilizando ÚNICAMENTE HTML5 semántico y CSS3 puro (sin una sola línea de JavaScript ni librerías externas).

--- ESTRUCTURA Y ARCHIVOS ---
1. Genera el código HTML con la arquitectura accesible.
2. Genera el código CSS en un bloque aparte, que luego guardaré como "estilosIA.css".
3. Las imágenes de las mascotas están ubicadas en la carpeta "imagenes/" y los archivos PDF de información en la carpeta "info/".

--- LISTADO DE MASCOTAS Y DATOS ESPECÍFICOS ---
Debes usar de forma exacta los siguientes datos para armar las tarjetas del listado:

Categoría: PERROS
1. Kira (Perra):
   - Imagen: "imagenes/perra_kira.png" (o JPG según corresponda)
   - PDF: "info/ficha_perra_kira.pdf"
   - Descripción corta: Perra dorada, alegre, dócil y sociable, de 3 años de edad.
2. Lola (Perra):
   - Imagen: "imagenes/perra_lola.png"
   - PDF: "info/ficha_perra_lola.pdf"
   - Descripción corta: Perrita joven blanca y canela, vivaz, juguetona y enérgica, de 1 año de edad.
3. Bruno (Perro):
   - Imagen: "imagenes/perro_bruno.png"
   - PDF: "info/ficha_perro_bruno.pdf"
   - Descripción corta: Labrador negro adulto, equilibrado, dócil y muy compañero, de 6 años de edad.

Categoría: GATOS
1. Nala (Gata):
   - Imagen: "imagenes/gata_nala.png"
   - PDF: "info/ficha_gata_nala.pdf"
   - Descripción corta: Gata blanco y negro de carácter sereno, tranquila y cariñosa, de 4 años de edad.
2. Milo (Gato):
   - Imagen: "imagenes/gato_milo.png"
   - PDF: "info/ficha_gato_milo.pdf"
   - Descripción corta: Gato atigrado naranja, curioso, activo y muy sociable, de 2 años de edad.
3. Simón (Gato):
   - Imagen: "imagenes/gato_simon.png"
   - PDF: "info/ficha_gato_simon.pdf"
   - Descripción corta: Gato gris de pelo largo, manso, afectuoso y de energía baja, de 7 años de edad.

--- REQUERIMIENTOS DEL ENUNCIADO ---
1. Navegación principal (<nav>) con enlaces a:
   - Formulario de contacto (campos semánticos con labels bien asociados).
   - Información de la persona/entidad que mantiene el sitio.
   - Listado de mascotas perdidas.
2. Filtrado dinámico sin JavaScript:
   - Permite seleccionar la categoría (Perros / Gatos / Ver Todos) usando <input type="radio"> ocultos combinados con CSS (selectores :checked).
3. Estilos de las tarjetas e imágenes:
   - Todas las fotos de las mascotas deben tener un marco uniforme con borde y relleno especificado mediante CSS. Las imágenes deben ser contain.
   - Incluye el enlace "+ Info" apuntando al PDF correspondiente en la carpeta "info/".
4. Diseños y maquetación:
   - Completamente responsivo (Media Queries).

--- ACCESIBILIDAD Y ARIA (ÉNFASIS ESPECIAL) ---
- Avisos a lectores de pantalla: Como el cambio de filtro es estático (vía CSS), configura atributos ARIA o zonas aria-live / role="status" / role="region" adecuadamente para que un lector de pantalla (como NVDA o JAWS) se entere cuando se cambia el filtro seleccionado o el contenido dinámico.
- Controles accesibles: Aplica `aria-controls`, `aria-checked` o etiquetas `<label>` bien configuradas para los radio buttons de filtrado.
- Textos alternativos (alt): Proporciona explicaciones claras en las imágenes usando la información de cada mascota (ej: "Foto de Bruno, labrador negro adulto").
- Enlaces accesibles: Asegúrate de que el texto accesible en "+ Info" proporcione contexto completo (ej: "+ Info - Ver ficha en PDF de Bruno").
- Navegación por teclado: Los controles de filtrado deben ser navegables y accionables con Tab y Espacio/Enter, manteniendo un estilo :focus bien visible.

Genera el código HTML y CSS en bloques de código separados de manera clara.
