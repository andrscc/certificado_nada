<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Certificado Oficial de Suministro de Nada Absoluta</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <script src="https://cdn.jsdelivr.net/npm/chart.js"></script>
    <!-- Visualization & Content Choices:
    - Certificate Title & Doc No: Inform -> Prominent H1/H2 -> Static -> Clear identification -> HTML/Tailwind.
    - Preamble & Articles: Inform -> Paragraphs and lists within styled sections/cards -> Static or subtle hover highlight -> Readability and structure -> HTML/Tailwind.
    - Commitments List (Article 3): Organize/Inform -> Ordered list within its section -> Static -> Clear presentation of duties -> HTML/Tailwind.
    - Signatures/Seal: Inform/Authenticate (humorous) -> Styled text blocks and a CSS-created seal placeholder -> Static -> Mimics official document -> HTML/Tailwind, Unicode/CSS for seal.
    - 'Verify' button: Engage/Humor -> Button -> onClick shows modal -> Enhances official parody -> JS for modal.
    - 'Print' button: Utility -> Button -> onClick triggers browser print -> Practical affordance -> JS for print.
    CONFIRMING NO SVG/Mermaid. All visual elements (lines, seal placeholder) via HTML/CSS. -->
    <style>
        @import url('https://fonts.googleapis.com/css2?family=EB+Garamond:ital,wght@0,400..800;1,400..800&family=Roboto:wght@300;400;700&display=swap');
        body {
            font-family: 'Roboto', sans-serif;
            background-color: #fdfbf5; /* Warm Neutral - Tailwind bg-amber-50 or similar */
            color: #374151; /* Tailwind text-gray-700 */
        }
        .certificate-font {
            font-family: 'EB Garamond', serif;
        }
        .accent-color {
            color: #b45309; /* Tailwind amber-700 */
        }
        .accent-bg {
            background-color: #b45309; /* Tailwind amber-700 */
        }
        .accent-border {
            border-color: #b45309; /* Tailwind amber-700 */
        }
        .btn-primary {
            @apply bg-amber-600 hover:bg-amber-700 text-white font-semibold py-2 px-4 rounded-lg shadow-md transition-colors duration-300;
        }
        .btn-secondary {
            @apply bg-stone-200 hover:bg-stone-300 text-stone-700 font-semibold py-2 px-4 rounded-lg shadow-md transition-colors duration-300;
        }
        .modal {
            display: none; /* Hidden by default */
            position: fixed;
            z-index: 1000;
            left: 0;
            top: 0;
            width: 100%;
            height: 100%;
            overflow: auto;
            background-color: rgba(0,0,0,0.5);
        }
        .modal-content {
            background-color: #fff;
            margin: 15% auto;
            padding: 20px;
            border: 1px solid #888;
            width: 80%;
            max-width: 500px;
            border-radius: 8px;
            text-align: center;
            box-shadow: 0 4px 8px 0 rgba(0,0,0,0.2),0 6px 20px 0 rgba(0,0,0,0.19);
        }
        .close-button {
            color: #aaa;
            float: right;
            font-size: 28px;
            font-weight: bold;
        }
        .close-button:hover,
        .close-button:focus {
            color: black;
            text-decoration: none;
            cursor: pointer;
        }
        .improved-seal {
            width: 100px;
            height: 100px;
            background-color: #c2410c; /* Tailwind orange-700 - a bit richer for a seal */
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            position: relative;
            box-shadow: 0px 2px 4px rgba(0,0,0,0.3), inset 0px 0px 10px rgba(0,0,0,0.2);
            border: 3px solid #9a3412; /* Tailwind orange-800 */
        }
        .improved-seal::before {
            content: '';
            position: absolute;
            width: 80%;
            height: 80%;
            border: 2px dashed #fbbf24; /* Tailwind amber-400 */
            border-radius: 50%;
            box-sizing: border-box;
        }
        .seal-text {
            font-family: 'EB Garamond', serif;
            font-size: 28px;
            font-weight: bold;
            color: #fef3c7; /* Tailwind amber-100 */
            position: relative; /* To ensure it's above the ::before pseudo-element */
            z-index: 1;
        }
    </style>
</head>
<body class="antialiased">

    <div class="container mx-auto p-4 sm:p-8 max-w-4xl certificate-font">
        <header class="text-center mb-10 mt-6">
            <h1 class="text-3xl sm:text-4xl font-bold accent-color tracking-wider">CERTIFICADO OFICIAL DE SUMINISTRO DE NADA ABSOLUTA</h1>
            <p class="text-lg text-gray-600 mt-2">Documento Nro: NADA-EXP-001-VDCP-AC</p>
        </header>

        <hr class="border-t-2 accent-border my-8">

        <section id="introduction" class="mb-8 bg-white p-6 rounded-lg shadow-lg">
            <h2 class="text-xl font-semibold mb-3 accent-color">Preámbulo del Certificado</h2>
            <p class="text-gray-700 leading-relaxed">
                Este documento interactivo presenta el "Certificado Oficial de Suministro de Nada Absoluta", una formalización única de un regalo muy especial. Navegue a través de sus secciones para conocer todos los detalles de este acuerdo trascendental. Cada artículo ha sido cuidadosamente redactado para garantizar la entrega impecable de... absolutamente nada.
            </p>
        </section>

        <main class="space-y-6">
            <article id="article1" class="bg-white p-6 rounded-lg shadow-lg hover:shadow-xl transition-shadow duration-300">
                <h3 class="text-xl font-semibold mb-3 accent-color">Artículo 1: Identificación de las Partes Contratantes</h3>
                <ul class="list-disc list-inside text-gray-700 space-y-1 pl-4">
                    <li><strong>Beneficiaria Designada de la Nada (en adelante "La Receptora"):</strong> V. D. C. P.</li>
                    <li><strong>Proveedor Certificado del Servicio de Nada (en adelante "El Garante del Vacío"):</strong> A. C.</li>
                </ul>
            </article>

            <article id="article2" class="bg-white p-6 rounded-lg shadow-lg hover:shadow-xl transition-shadow duration-300">
                <h3 class="text-xl font-semibold mb-3 accent-color">Artículo 2: Objeto del Certificado</h3>
                <p class="text-gray-700 leading-relaxed">
                    El Garante del Vacío se compromete a suministrar a La Receptora <strong>UNA (1) HORA CRONOMETRADA</strong>, indivisible e ininterrumpida, de <strong>NADA ABSOLUTA</strong> (en adelante "La Experiencia"). Dicha Experiencia se define como un periodo exento de estímulos externos, responsabilidades, interacciones no solicitadas y cualquier otra manifestación del "algo" que pueda perturbar el estado de pura inactividad.
                </p>
            </article>

            <article id="article3" class="bg-white p-6 rounded-lg shadow-lg hover:shadow-xl transition-shadow duration-300">
                <h3 class="text-xl font-semibold mb-3 accent-color">Artículo 3: Compromisos Esenciales del Garante del Vacío</h3>
                <p class="text-gray-700 leading-relaxed mb-2">
                    Para la correcta materialización de La Experiencia, El Garante del Vacío se obliga a:
                </p>
                <ol class="list-decimal list-inside text-gray-700 space-y-2 pl-4">
                    <li><strong>Implementación del Protocolo de Aislamiento Sensorial Avanzado:</strong> Neutralización sistemática de todos los dispositivos electrónicos susceptibles de emitir notificaciones (teléfonos móviles, tabletas, ordenadores, asistentes virtuales) en el perímetro designado para La Experiencia. Esto podrá incluir la reubicación temporal de dichos dispositivos o su encapsulamiento en un Dispositivo de Contención de Alertas (D.C.A.).</li>
                    <li><strong>Establecimiento de la "Zona de Serenidad Cero":</strong> Adecuación de un espacio físico (en adelante "El Santuario de Nada") para minimizar la contaminación lumínica y acústica. Se aplicarán medidas para mitigar el impacto de ruidos urbanos (considerando el entorno de Caracas) y otros factores ambientales perturbadores.</li>
                    <li><strong>Defensa Activa Contra el "Algo":</strong> El Garante del Vacío ejercerá una vigilancia discreta y perimetral al Santuario de Nada, interceptando y gestionando cualquier intento de incursión por parte de estímulos externos, incluyendo, pero no limitándose a: timbres, llamadas a la puerta, fauna doméstica curiosa u otros cohabitantes no involucrados en La Experiencia.</li>
                    <li><strong>Garantía de No Interferencia Propia:</strong> El Garante del Vacío se abstendrá de cualquier comunicación o interacción con La Receptora durante el transcurso de La Experiencia, salvo en caso de emergencia que ponga en riesgo la integridad conceptual de la "nada" (situación altamente improbable según nuestros análisis de riesgo).</li>
                </ol>
            </article>

            <article id="article4" class="bg-white p-6 rounded-lg shadow-lg hover:shadow-xl transition-shadow duration-300">
                <h3 class="text-xl font-semibold mb-3 accent-color">Artículo 4: Condiciones de Canje y Validez</h3>
                <ul class="list-disc list-inside text-gray-700 space-y-1 pl-4">
                    <li>El presente Certificado es canjeable por La Receptora en una fecha y hora de mutuo acuerdo con El Garante del Vacío, notificándose con una antelación mínima de veinticuatro (24) horas para permitir la adecuada preparación logística y ambiental.</li>
                    <li>La validez de este Certificado es de sesenta (60) días naturales a partir de la fecha de emisión, para asegurar que La Experiencia se disfrute en su punto óptimo de "nadidad".</li>
                </ul>
            </article>

            <article id="article5" class="bg-white p-6 rounded-lg shadow-lg hover:shadow-xl transition-shadow duration-300">
                <h3 class="text-xl font-semibold mb-3 accent-color">Artículo 5: Disposiciones Finales</h3>
                <p class="text-gray-700 leading-relaxed">
                    Este Certificado representa la totalidad del acuerdo entre las partes con respecto a la provisión de La Experiencia. Cualquier modificación deberá ser acordada por escrito. Se espera que La Receptora se aproxime a La Experiencia con una mente abierta a la potencialidad del vacío.
                </p>
            </article>

        </main>

        <hr class="border-t-2 accent-border my-8">

        <footer class="text-center mt-10 mb-10">
            <p class="text-lg text-gray-600 mb-6"><strong>Lugar y Fecha de Emisión:</strong> Caracas, 30 de mayo de 2025.</p>

            <div class="flex flex-col sm:flex-row justify-around items-center space-y-8 sm:space-y-0 sm:space-x-6">
                <div class="seal-area text-center flex flex-col items-center">
                    <div class="improved-seal" title="Sello Oficial de Asuntos Intangibles y Experiencias Nulas">
                        <span class="seal-text">OAIEN</span>
                    </div>
                    <p class="text-xs text-gray-500 mt-2">(Sello de la Oficina de Asuntos Intangibles y Experiencias Nulas)</p>
                </div>

                <div class="signatures-area space-y-6 w-full sm:w-auto">
                    <div class="signature-block">
                        <div class="w-60 h-8 border-b-2 border-gray-400 mx-auto"></div>
                        <p class="mt-1 text-sm text-gray-700">V. D. C. P.</p>
                        <p class="text-xs text-gray-500">(La Receptora)</p>
                        <p class="text-xs text-gray-500 italic">"Acepto solemnemente recibir Nada"</p>
                    </div>
                    <div class="signature-block">
                        <div class="w-60 h-8 border-b-2 border-gray-400 mx-auto"></div>
                        <p class="mt-1 text-sm text-gray-700">A. C.</p>
                        <p class="text-xs text-gray-500">(El Garante del Vacío)</p>
                        <p class="text-xs text-gray-500 italic">"Me comprometo formalmente a proveer Nada"</p>
                    </div>
                </div>
            </div>
        </footer>

        <div class="text-center my-10 space-x-4">
            <button id="verifyButton" class="btn-primary">Verificar Certificado</button>
            <button onclick="window.print()" class="btn-secondary">Imprimir Certificado</button>
        </div>
    </div>

    <div id="verificationModal" class="modal">
        <div class="modal-content">
            <span class="close-button" onclick="closeModal()">&times;</span>
            <h3 class="text-xl font-semibold mb-3 accent-color">Verificación de Autenticidad</h3>
            <p class="text-gray-700">Este certificado ha sido verificado y es auténtico.</p>
            <p class="text-gray-600 mt-2">¡La provisión de "Nada Absoluta" está garantizada por El Garante del Vacío!</p>
            <button onclick="closeModal()" class="btn-primary mt-4">Entendido</button>
        </div>
    </div>

    <script>
        // Modal JavaScript
        const modal = document.getElementById('verificationModal');
        const verifyButton = document.getElementById('verifyButton');

        if (verifyButton) {
            verifyButton.onclick = function() {
                if(modal) modal.style.display = "block";
            }
        }
        
        function closeModal() {
            if(modal) modal.style.display = "none";
        }

        window.onclick = function(event) {
            if (event.target == modal) {
                if(modal) modal.style.display = "none";
            }
        }

        // Placeholder chart logic is removed as per request.
        // Chart.js script tag is kept as per original requirements, even if not actively used now.
    </script>
</body>
</html>
