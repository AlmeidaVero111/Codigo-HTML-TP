# Codigo-HTML-TP
Trabajo Práctico de Diseño de Interfaces - Laboratorio de Analisis Clinicos
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <title>Interfaces Lab - Nivel Básico</title>
</head>
<body>

    <!-- TÍTULO PRINCIPAL -->
    <h1>Sistema de Laboratorio de Análisis Clínicos</h1>
    <hr>

    <!-- ==================================================================================== -->
    <!-- 1. FORMULARIO DE CARGA DE INFORME -->
    <!-- Etiquetas clave: form, h2, label, input, button -->
    <!-- ==================================================================================== -->
    <h2>1. Formulario de Carga de Nuevo Informe (Borrador)</h2>
    <form action="#" method="POST">
        
        <!-- DATOS DEL PACIENTE -->
        <h3>Datos del Paciente</h3>
        <label for="dni">DNI:</label>
        <input type="text" id="dni" required><br>

        <label for="paciente_nombre">Nombre y Apellido:</label>
        <input type="text" id="paciente_nombre" required><br>

        <label for="paciente_os">Obra Social Primaria:</label>
        <input type="text" id="paciente_os"><br>
        <p>... más datos del paciente (fecha nacimiento, contacto, etc.)</p>

        <!-- DATOS DEL MÉDICO SOLICITANTE -->
        <h3>Datos del Médico Solicitante</h3>
        <label for="solicitante_mp">Matrícula Profesional (MP):</label>
        <input type="text" id="solicitante_mp" required><br>

        <label for="solicitante_nombre">Institución/Procedencia:</label>
        <input type="text" id="solicitante_nombre"><br>
        
        <!-- PRÁCTICAS SOLICITADAS (Tabla para estructura de detalle) -->
        <h3>Prácticas Solicitadas</h3>
        <table>
            <thead>
                <tr>
                    <th>Código Nomenclador</th>
                    <th>Descripción</th>
                    <th>Muestra Remitida</th>
                </tr>
            </thead>
            <tbody>
                <tr>
                    <!-- Campos vacíos listos para la entrada de datos -->
                    <td><input type="text"></td>
                    <td><input type="text"></td>
                    <td><input type="text"></td>
                </tr>
            </tbody>
        </table>

        <p style="color: red;">Estado Inicial: Borrador</p>
        <button type="submit">Guardar Informe</button>
    </form>
    <hr>


    <!-- ==================================================================================== -->
    <!-- 2. PANTALLA DE BÚSQUEDA -->
    <!-- Etiquetas clave: h2, form, label, select, table -->
    <!-- ==================================================================================== -->
    <h2>2. Pantalla de Búsqueda de Informes</h2>
    <form action="#" method="GET">
        <h3>Criterios de Búsqueda</h3>
        <label for="search_nro">N° de Informe:</label>
        <input type="text" id="search_nro"><br>

        <label for="search_estado">Estado:</label>
        <select id="search_estado">
            <option value="revision">En Revisión Profesional</option>
            <option value="borrador">Borrador</option>
        </select><br>
        
        <button type="submit">Buscar</button>
    </form>

    <h3>Resultados de la Búsqueda</h3>
    <table>
        <thead>
            <tr>
                <th>N° Informe</th>
                <th>Paciente</th>
                <th>Estado</th>
                <th>Acción</th>
            </tr>
        </thead>
        <tbody>
            <tr>
                <!-- Fila de ejemplo vacía para mostrar la estructura -->
                <td>_________</td>
                <td>_________</td>
                <td>_________</td>
                <td><a href="#">Abrir</a></td>
            </tr>
        </tbody>
    </table>
    <hr>


    <!-- ==================================================================================== -->
    <!-- 3. INFORME POR PANTALLA (VISTA DETALLE) -->
    <!-- Se usa "______" para simular la línea punteada en datos estáticos -->
    <!-- ==================================================================================== -->
    <h2>3. Vista Detalle del Informe Bioquímico</h2>
    
    <!-- ENCABEZADO FIJO -->
    <header>
        <h3>LABORATORIO CENTRAL BIO</h3>
        <p>Domicilio: ________________ | Contacto: ________________</p>
    </header>
    
    <!-- ENCABEZADO VARIABLE (MAESTRO) -->
    <section>
        <h4>Datos del Informe</h4>
        <p><strong>N° Informe:</strong> ________ | <strong>Estado:</strong> ________</p>
        <p><strong>Paciente:</strong> ________ | <strong>DNI:</strong> ________ | <strong>Edad:</strong> ________</p>
        <p><strong>Profesional Lab:</strong> ________ | <strong>Solicitante:</strong> ________</p>
    </section>

    <!-- DETALLE DEL INFORME (Tabla de resultados con placeholders) -->
    <section>
        <h4>Detalle de Prácticas y Resultados</h4>
        <table>
            <thead>
                <tr>
                    <th>Muestra</th>
                    <th>Estudio</th>
                    <th>Valor Encontrado</th>
                    <th>Valor de Referencia</th>
                    <th>Observaciones</th>
                </tr>
            </thead>
            <tbody>
                <tr>
                    <td>_________</td>
                    <td>_________</td>
                    <td>_________</td>
                    <td>_________</td>
                    <td>_________</td>
                </tr>
            </tbody>
        </table>
    </section>

    <!-- PIE DE INFORME -->
    <footer>
        <p style="text-align: right;">Generado: ________ | Página ________ de ________</p>
    </footer>

</body>
</html>
