# FORMULARIO_INCENDIOS
QUESTIONARIO DE EVALUACIÓN DE INCENDIOS EN VIVIENDAS DE INTERCIFIE URBANA FORESTAL
<!DOCTYPE html>
<!-- saved from url=(0061)file:///C:/Users/6736.aripoll_a.cifpj/Downloads/!DOCTYPE.html -->
<html lang="ca"><head><meta http-equiv="Content-Type" content="text/html; charset=UTF-8">
    
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Qüestionari d'Avaluació del Risc d'Incendi en Edificacions</title>
    <style>
        /* Estils per a format DIN A4 - UNA SOLA PÀGINA */
        @page {
            size: A4;
            margin: 10mm 15mm;
        }
        
        body {
            font-family: 'Arial', sans-serif;
            font-size: 9.5px;
            line-height: 1.2;
            color: #000;
            background: white;
            margin: 0;
            padding: 0;
            width: 210mm;
            min-height: 297mm;
            box-sizing: border-box;
        }
        
        .a4-container {
            width: 210mm;
            min-height: 277mm; /* 297mm - marges superior/inferior */
            padding: 5mm 10mm;
            box-sizing: border-box;
            background: white;
        }
        
        /* Capçalera */
        .header {
            text-align: center;
            margin-bottom: 8px;
            padding-bottom: 5px;
            border-bottom: 1.5px solid #333;
        }
        
        .header h1 {
            font-size: 14px;
            margin: 0 0 3px 0;
            color: #333;
            font-weight: bold;
        }
        
        .header h2 {
            font-size: 10px;
            margin: 0;
            color: #666;
            font-weight: normal;
        }
        
        /* Taula principal compacta */
        .main-table {
            width: 100%;
            border-collapse: collapse;
            margin-bottom: 5px;
            table-layout: fixed;
            font-size: 9px;
        }
        
        .main-table th,
        .main-table td {
            border: 0.5px solid #999;
            padding: 4px 5px;
            vertical-align: top;
            text-align: left;
        }
        
        .main-table th {
            background-color: #f5f5f5;
            font-weight: bold;
            text-align: center;
        }
        
        /* Columnes optimitzades per a una pàgina */
        .col-apartat { 
            width: 10%;
            font-weight: bold;
            text-align: center;
        }
        
        .col-item { 
            width: 20%;
        }
        
        .col-opcions { 
            width: 55%;
        }
        
        .col-punts { 
            width: 15%;
            text-align: center;
        }
        
        /* Grups d'opcions compactes */
        .option-line {
            margin-bottom: 2px;
            display: flex;
            align-items: flex-start;
            page-break-inside: avoid;
        }
        
        .option-line.last {
            margin-bottom: 0;
        }
        
        /* Checkboxes i labels compactes */
        .checkbox-group {
            display: inline-flex;
            align-items: center;
            margin-right: 12px;
            white-space: nowrap;
        }
        
        input[type="checkbox"] {
            margin-right: 3px;
            transform: scale(0.8);
            vertical-align: middle;
        }
        
        .option-label {
            font-size: 8.5px;
            margin-right: 3px;
        }
        
        .punt-value {
            font-weight: bold;
            color: #d32f2f;
            font-size: 8.5px;
            margin-left: auto;
        }
        
        /* Inputs de text compactes */
        .text-input {
            border: none;
            border-bottom: 0.5px solid #999;
            background: transparent;
            width: 70px;
            font-size: 9px;
            padding: 1px 2px;
            margin: 0 3px;
        }
        
        .text-input.small {
            width: 50px;
        }
        
        /* Secció de síntesi compacta */
        .synthesis-section {
            margin-top: 8px;
            border: 1.5px solid #333;
            padding: 6px;
            page-break-inside: avoid;
            background-color: #fafafa;
        }
        
        .synthesis-title {
            font-size: 10px;
            font-weight: bold;
            text-align: center;
            margin: 0 0 5px 0;
            color: #333;
        }
        
        .synthesis-grid {
            display: grid;
            grid-template-columns: repeat(5, 1fr);
            gap: 5px;
            margin-bottom: 5px;
        }
        
        .synthesis-item {
            text-align: center;
        }
        
        .synthesis-label {
            font-size: 8.5px;
            font-weight: bold;
            margin-bottom: 2px;
        }
        
        .score-input {
            width: 40px;
            height: 20px;
            border: 1px solid #999;
            text-align: center;
            font-weight: bold;
            font-size: 10px;
            margin: 0 auto;
            display: block;
            background-color: white;
        }
        
        .total-box {
            grid-column: span 5;
            text-align: center;
            padding-top: 3px;
            border-top: 1px dashed #999;
            margin-top: 3px;
        }
        
        .total-label {
            font-size: 10px;
            font-weight: bold;
            margin-right: 10px;
        }
        
        #total_general {
            width: 60px;
            height: 24px;
            font-size: 12px;
            background-color: #fff8e1;
        }
        
        /* Interpretació compacta */
        .interpretation {
            margin-top: 5px;
            padding: 4px;
            border: 1px solid #ddd;
            background-color: white;
        }
        
        .interpretation-title {
            font-size: 9px;
            font-weight: bold;
            margin-bottom: 3px;
            color: #555;
        }
        
        .interpretation-grid {
            display: grid;
            grid-template-columns: repeat(2, 1fr);
            gap: 3px;
        }
        
        .interpretation-item {
            font-size: 8.5px;
            display: flex;
            align-items: center;
        }
        
        .interpretation-checkbox {
            margin-right: 4px;
            transform: scale(0.7);
        }
        
        /* Colors per a nivells de risc */
        .risk-low { color: #2e7d32; }
        .risk-moderate { color: #f57c00; }
        .risk-high { color: #d32f2f; }
        .risk-extreme { color: #b71c1c; }
        
        /* Utilitats */
        .subtotal-row td {
            background-color: #e8f5e9 !important;
            font-weight: bold;
            font-size: 9px;
        }
        
        .section-title {
            font-weight: bold;
            background-color: #f0f0f0;
            font-size: 9.5px;
        }
        
        .note {
            font-size: 8px;
            color: #777;
            font-style: italic;
            margin-top: 2px;
        }
        
        /* Per a la impressió */
        @media print {
            body {
                width: 210mm;
                height: 297mm;
                background: white;
                font-size: 9px;
            }
            
            .a4-container {
                padding: 5mm 10mm;
                margin: 0;
            }
            
            .no-print {
                display: none;
            }
            
            .score-input {
                border: 0.5px solid #999;
                -webkit-print-color-adjust: exact;
            }
            
            .checkbox-group {
                -webkit-print-color-adjust: exact;
            }
        }
        
        /* Controls no imprimibles */
        .controls {
            position: fixed;
            bottom: 15px;
            right: 15px;
            background: white;
            padding: 8px;
            border: 1px solid #ccc;
            border-radius: 4px;
            box-shadow: 0 2px 6px rgba(0,0,0,0.1);
            z-index: 1000;
            font-size: 10px;
        }
        
        .controls button {
            margin: 0 4px;
            padding: 5px 10px;
            background: #2196F3;
            color: white;
            border: none;
            border-radius: 2px;
            cursor: pointer;
            font-size: 10px;
        }
        
        .controls button:hover {
            background: #1976D2;
        }
        
        /* Estils per a files específiques */
        .compact-options {
            display: flex;
            flex-wrap: wrap;
            gap: 2px 8px;
        }
    </style>
</head>
<body>
    <div class="a4-container">
        <div class="header">
            <h1>QÜESTIONARI D'AVALUACIÓ DEL RISC D'INCENDI EN EDIFICACIONS</h1>
            <h2>Document únic d'avaluació - Versió compacta</h2>
        </div>
        
        <!-- Taula principal - TOT EN UNA PÀGINA -->
        <table class="main-table">
            <thead>
                <tr>
                    <th class="col-apartat">APARTAT</th>
                    <th class="col-item">ÍTEM</th>
                    <th class="col-opcions">OPCIONS</th>
                    <th class="col-punts">PUNTS</th>
                </tr>
            </thead>
            <tbody>
                <!-- DADES GENERALS -->
                <tr class="section-title">
                    <td class="col-apartat">DADES<br>GENERALS</td>
                    <td>Urbanització</td>
                    <td>
                        <input type="text" class="text-input" placeholder="Nom urbanització/municipi">
                    </td>
                    <td>—</td>
                </tr>
                <tr>
                    <td></td>
                    <td>Municipi</td>
                    <td>
                        <input type="text" class="text-input" placeholder="Terme municipal">
                    </td>
                    <td>—</td>
                </tr>
                <tr>
                    <td></td>
                    <td>Propietari</td>
                    <td>
                        <div class="compact-options">
                            <div class="checkbox-group">
                                <input type="checkbox" id="prop_resident" class="interpretation-checkbox">
                                <label for="prop_resident" class="option-label">Resident</label>
                            </div>
                            <div class="checkbox-group">
                                <input type="checkbox" id="prop_estranger" class="interpretation-checkbox">
                                <label for="prop_estranger" class="option-label">Estranger</label>
                            </div>
                        </div>
                    </td>
                    <td>—</td>
                </tr>
                <tr>
                    <td></td>
                    <td>Nacionalitat</td>
                    <td>
                        <div class="compact-options">
                            <div class="checkbox-group">
                                <input type="checkbox" id="nac_espanyol" class="interpretation-checkbox">
                                <label for="nac_espanyol" class="option-label">Espanyol</label>
                            </div>
                            <div class="checkbox-group">
                                <input type="checkbox" id="nac_stranger" class="interpretation-checkbox">
                                <label for="nac_stranger" class="option-label">Estranger:</label>
                                <input type="text" class="text-input small" placeholder="País">
                            </div>
                        </div>
                    </td>
                    <td>—</td>
                </tr>
                <tr>
                    <td></td>
                    <td>Entrevistat</td>
                    <td>
                        <div class="compact-options">
                            <div class="checkbox-group">
                                <input type="checkbox" id="entrev_home" class="interpretation-checkbox">
                                <label for="entrev_home" class="option-label">Home (H)</label>
                            </div>
                            <div class="checkbox-group">
                                <input type="checkbox" id="entrev_dona" class="interpretation-checkbox">
                                <label for="entrev_dona" class="option-label">Dona (D)</label>
                            </div>
                        </div>
                    </td>
                    <td>—</td>
                </tr>
                
                <!-- APARTAT A -->
                <tr class="section-title">
                    <td class="col-apartat">A<br>PREVENCIÓ</td>
                    <td>Estat prevenció</td>
                    <td>
                        <div class="option-line">
                            <div class="checkbox-group">
                                <input type="checkbox" id="a1_1" class="option-checkbox">
                                <label for="a1_1" class="option-label">&gt;3 anys</label>
                                <span class="punt-value">(4)</span>
                            </div>
                            <div class="checkbox-group">
                                <input type="checkbox" id="a1_2" class="option-checkbox">
                                <label for="a1_2" class="option-label">1-3 anys</label>
                                <span class="punt-value">(2)</span>
                            </div>
                            <div class="checkbox-group">
                                <input type="checkbox" id="a1_3" class="option-checkbox">
                                <label for="a1_3" class="option-label">Anual</label>
                                <span class="punt-value">(0)</span>
                            </div>
                        </div>
                    </td>
                    <td>
                        <input type="text" class="score-input" id="puntuacio_a1" value="0" readonly="">
                    </td>
                </tr>
                <tr>
                    <td></td>
                    <td>Coneixement</td>
                    <td>
                        <div class="option-line">
                            <div class="checkbox-group">
                                <input type="checkbox" id="a2_1" class="option-checkbox">
                                <label for="a2_1" class="option-label">Gens</label>
                                <span class="punt-value">(2)</span>
                            </div>
                            <div class="checkbox-group">
                                <input type="checkbox" id="a2_2" class="option-checkbox">
                                <label for="a2_2" class="option-label">Mig</label>
                                <span class="punt-value">(1)</span>
                            </div>
                            <div class="checkbox-group">
                                <input type="checkbox" id="a2_3" class="option-checkbox">
                                <label for="a2_3" class="option-label">Alt</label>
                                <span class="punt-value">(0)</span>
                            </div>
                        </div>
                    </td>
                    <td>
                        <input type="text" class="score-input" id="puntuacio_a2" value="0" readonly="">
                    </td>
                </tr>
                <tr class="subtotal-row">
                    <td colspan="3">SUBTOTAL APARTAT A →</td>
                    <td><input type="text" class="score-input" id="subtotal_a" value="0" readonly=""></td>
                </tr>
                
                <!-- APARTAT B -->
                <tr class="section-title">
                    <td class="col-apartat">B<br>VEGETACIÓ</td>
                    <td>Tipus vegetació</td>
                    <td>
                        <div class="option-line">
                            <div class="compact-options">
                                <div class="checkbox-group">
                                    <input type="checkbox" id="b1_1" class="option-checkbox">
                                    <label for="b1_1" class="option-label">Coníferes (Con)</label>
                                    <span class="punt-value">(4)</span>
                                </div>
                                <div class="checkbox-group">
                                    <input type="checkbox" id="b1_2" class="option-checkbox">
                                    <label for="b1_2" class="option-label">Arbustives (Arb)</label>
                                    <span class="punt-value">(3)</span>
                                </div>
                                <div class="checkbox-group">
                                    <input type="checkbox" id="b1_3" class="option-checkbox">
                                    <label for="b1_3" class="option-label">Frondoses (Fro)</label>
                                    <span class="punt-value">(2)</span>
                                </div>
                                <div class="checkbox-group">
                                    <input type="checkbox" id="b1_4" class="option-checkbox">
                                    <label for="b1_4" class="option-label">Pastura (Pas)</label>
                                    <span class="punt-value">(1)</span>
                                </div>
                                <div class="checkbox-group">
                                    <input type="checkbox" id="b1_5" class="option-checkbox">
                                    <label for="b1_5" class="option-label">Sòl nu (Nu)</label>
                                    <span class="punt-value">(0)</span>
                                </div>
                            </div>
                        </div>
                    </td>
                    <td>
                        <input type="text" class="score-input" id="puntuacio_b1" value="0" readonly="">
                    </td>
                </tr>
                <tr>
                    <td></td>
                    <td>Estructura</td>
                    <td>
                        <div class="option-line">
                            <div class="compact-options">
                                <div class="checkbox-group">
                                    <input type="checkbox" id="b2_1" class="option-checkbox">
                                    <label for="b2_1" class="option-label">Alta</label>
                                    <span class="punt-value">(3)</span>
                                </div>
                                <div class="checkbox-group">
                                    <input type="checkbox" id="b2_2" class="option-checkbox">
                                    <label for="b2_2" class="option-label">Mitjana (Mitj)</label>
                                    <span class="punt-value">(2)</span>
                                </div>
                                <div class="checkbox-group">
                                    <input type="checkbox" id="b2_3" class="option-checkbox">
                                    <label for="b2_3" class="option-label">Baixa</label>
                                    <span class="punt-value">(1)</span>
                                </div>
                                <div class="checkbox-group">
                                    <input type="checkbox" id="b2_4" class="option-checkbox">
                                    <label for="b2_4" class="option-label">Clara</label>
                                    <span class="punt-value">(0)</span>
                                </div>
                            </div>
                        </div>
                    </td>
                    <td>
                        <input type="text" class="score-input" id="puntuacio_b2" value="0" readonly="">
                    </td>
                </tr>
                <tr>
                    <td></td>
                    <td>Distància</td>
                    <td>
                        <div class="option-line">
                            <div class="compact-options">
                                <div class="checkbox-group">
                                    <input type="checkbox" id="b3_1" class="option-checkbox">
                                    <label for="b3_1" class="option-label">Contacte</label>
                                    <span class="punt-value">(3)</span>
                                </div>
                                <div class="checkbox-group">
                                    <input type="checkbox" id="b3_2" class="option-checkbox">
                                    <label for="b3_2" class="option-label">&gt;5 m</label>
                                    <span class="punt-value">(1)</span>
                                </div>
                                <div class="checkbox-group">
                                    <input type="checkbox" id="b3_3" class="option-checkbox">
                                    <label for="b3_3" class="option-label">&gt;10 m</label>
                                    <span class="punt-value">(0)</span>
                                </div>
                            </div>
                        </div>
                    </td>
                    <td>
                        <input type="text" class="score-input" id="puntuacio_b3" value="0" readonly="">
                    </td>
                </tr>
                <tr class="subtotal-row">
                    <td colspan="3">SUBTOTAL APARTAT B →</td>
                    <td><input type="text" class="score-input" id="subtotal_b" value="0" readonly=""></td>
                </tr>
                
                <!-- APARTAT C -->
                <tr class="section-title">
                    <td class="col-apartat">C<br>ENTORN</td>
                    <td>Ubicació</td>
                    <td>
                        <div class="option-line">
                            <div class="compact-options">
                                <div class="checkbox-group">
                                    <input type="checkbox" id="c1_1" class="option-checkbox">
                                    <label for="c1_1" class="option-label">Fons de vall (Vall)</label>
                                    <span class="punt-value">(3)</span>
                                </div>
                                <div class="checkbox-group">
                                    <input type="checkbox" id="c1_2" class="option-checkbox">
                                    <label for="c1_2" class="option-label">Pendent &gt;10%</label>
                                    <span class="punt-value">(2)</span>
                                </div>
                                <div class="checkbox-group">
                                    <input type="checkbox" id="c1_3" class="option-checkbox">
                                    <label for="c1_3" class="option-label">Pendent &lt;10%</label>
                                    <span class="punt-value">(1)</span>
                                </div>
                                <div class="checkbox-group">
                                    <input type="checkbox" id="c1_4" class="option-checkbox">
                                    <label for="c1_4" class="option-label">Pla</label>
                                    <span class="punt-value">(0)</span>
                                </div>
                            </div>
                        </div>
                    </td>
                    <td>
                        <input type="text" class="score-input" id="puntuacio_c1" value="0" readonly="">
                    </td>
                </tr>
                <tr>
                    <td></td>
                    <td>Mobiliari</td>
                    <td>
                        <div class="option-line">
                            <div class="compact-options">
                                <div class="checkbox-group">
                                    <input type="checkbox" id="c2_1" class="option-checkbox">
                                    <label for="c2_1" class="option-label">PVC</label>
                                    <span class="punt-value">(2)</span>
                                </div>
                                <div class="checkbox-group">
                                    <input type="checkbox" id="c2_2" class="option-checkbox">
                                    <label for="c2_2" class="option-label">Fusta</label>
                                    <span class="punt-value">(1)</span>
                                </div>
                                <div class="checkbox-group">
                                    <input type="checkbox" id="c2_3" class="option-checkbox">
                                    <label for="c2_3" class="option-label">Pedra</label>
                                    <span class="punt-value">(0)</span>
                                </div>
                            </div>
                        </div>
                        <div class="option-line last">
                            <div class="compact-options">
                                <div class="checkbox-group">
                                    <input type="checkbox" id="c2_4" class="option-checkbox">
                                    <label for="c2_4" class="option-label">Tendal</label>
                                    <span class="punt-value">(2)</span>
                                </div>
                                <div class="checkbox-group">
                                    <input type="checkbox" id="c2_5" class="option-checkbox">
                                    <label for="c2_5" class="option-label">Barbacoa (BBQ)</label>
                                    <span class="punt-value">(3)</span>
                                </div>
                            </div>
                        </div>
                    </td>
                    <td>
                        <input type="text" class="score-input" id="puntuacio_c2" value="0" readonly="">
                    </td>
                </tr>
                <tr>
                    <td></td>
                    <td>Materials ext.</td>
                    <td>
                        <div class="option-line">
                            <div class="compact-options">
                                <div class="checkbox-group">
                                    <input type="checkbox" id="c3_1" class="option-checkbox">
                                    <label for="c3_1" class="option-label">Cap</label>
                                    <span class="punt-value">(0)</span>
                                </div>
                                <div class="checkbox-group">
                                    <input type="checkbox" id="c3_2" class="option-checkbox">
                                    <label for="c3_2" class="option-label">Pintures (Pint.)</label>
                                    <span class="punt-value">(4)</span>
                                </div>
                                <div class="checkbox-group">
                                    <input type="checkbox" id="c3_3" class="option-checkbox">
                                    <label for="c3_3" class="option-label">Gas</label>
                                    <span class="punt-value">(3)</span>
                                </div>
                                <div class="checkbox-group">
                                    <input type="checkbox" id="c3_4" class="option-checkbox">
                                    <label for="c3_4" class="option-label">Llenya</label>
                                    <span class="punt-value">(2)</span>
                                </div>
                            </div>
                        </div>
                    </td>
                    <td>
                        <input type="text" class="score-input" id="puntuacio_c3" value="0" readonly="">
                    </td>
                </tr>
                <tr>
                    <td></td>
                    <td>Dist. materials</td>
                    <td>
                        <div class="option-line">
                            <div class="compact-options">
                                <div class="checkbox-group">
                                    <input type="checkbox" id="c4_1" class="option-checkbox">
                                    <label for="c4_1" class="option-label">Contacte (Cont.)</label>
                                    <span class="punt-value">(3)</span>
                                </div>
                                <div class="checkbox-group">
                                    <input type="checkbox" id="c4_2" class="option-checkbox">
                                    <label for="c4_2" class="option-label">&lt;50 m</label>
                                    <span class="punt-value">(2)</span>
                                </div>
                                <div class="checkbox-group">
                                    <input type="checkbox" id="c4_3" class="option-checkbox">
                                    <label for="c4_3" class="option-label">&gt;50 m</label>
                                    <span class="punt-value">(0)</span>
                                </div>
                            </div>
                        </div>
                    </td>
                    <td>
                        <input type="text" class="score-input" id="puntuacio_c4" value="0" readonly="">
                    </td>
                </tr>
                <tr class="subtotal-row">
                    <td colspan="3">SUBTOTAL APARTAT C →</td>
                    <td><input type="text" class="score-input" id="subtotal_c" value="0" readonly=""></td>
                </tr>
                
                <!-- APARTAT D -->
                <tr class="section-title">
                    <td class="col-apartat">D<br>EDIFICACIÓ</td>
                    <td>Vies accés</td>
                    <td>
                        <div class="option-line">
                            <div class="compact-options">
                                <div class="checkbox-group">
                                    <input type="checkbox" id="d1_1" class="option-checkbox">
                                    <label for="d1_1" class="option-label">1 via</label>
                                    <span class="punt-value">(2)</span>
                                </div>
                                <div class="checkbox-group">
                                    <input type="checkbox" id="d1_2" class="option-checkbox">
                                    <label for="d1_2" class="option-label">&gt;1 via</label>
                                    <span class="punt-value">(0)</span>
                                </div>
                            </div>
                        </div>
                    </td>
                    <td>
                        <input type="text" class="score-input" id="puntuacio_d1" value="0" readonly="">
                    </td>
                </tr>
                <tr>
                    <td></td>
                    <td>Tancament</td>
                    <td>
                        <div class="option-line">
                            <div class="compact-options">
                                <div class="checkbox-group">
                                    <input type="checkbox" id="d2_1" class="option-checkbox">
                                    <label for="d2_1" class="option-label">Obert / reixa</label>
                                    <span class="punt-value">(3)</span>
                                </div>
                                <div class="checkbox-group">
                                    <input type="checkbox" id="d2_2" class="option-checkbox">
                                    <label for="d2_2" class="option-label">Bardissa</label>
                                    <span class="punt-value">(5)</span>
                                </div>
                                <div class="checkbox-group">
                                    <input type="checkbox" id="d2_3" class="option-checkbox">
                                    <label for="d2_3" class="option-label">Mur pedra/obra</label>
                                    <span class="punt-value">(0)</span>
                                </div>
                            </div>
                        </div>
                    </td>
                    <td>
                        <input type="text" class="score-input" id="puntuacio_d2" value="0" readonly="">
                    </td>
                </tr>
                <tr>
                    <td></td>
                    <td>Accés</td>
                    <td>
                        <div class="option-line">
                            <div class="compact-options">
                                <div class="checkbox-group">
                                    <input type="checkbox" id="d3_1" class="option-checkbox">
                                    <label for="d3_1" class="option-label">Automàtic (Auto)</label>
                                    <span class="punt-value">(2)</span>
                                </div>
                                <div class="checkbox-group">
                                    <input type="checkbox" id="d3_2" class="option-checkbox">
                                    <label for="d3_2" class="option-label">Manual</label>
                                    <span class="punt-value">(1)</span>
                                </div>
                                <div class="checkbox-group">
                                    <input type="checkbox" id="d3_3" class="option-checkbox">
                                    <label for="d3_3" class="option-label">Obert</label>
                                    <span class="punt-value">(0)</span>
                                </div>
                            </div>
                        </div>
                    </td>
                    <td>
                        <input type="text" class="score-input" id="puntuacio_d3" value="0" readonly="">
                    </td>
                </tr>
                <tr class="subtotal-row">
                    <td colspan="3">SUBTOTAL APARTAT D →</td>
                    <td><input type="text" class="score-input" id="subtotal_d" value="0" readonly=""></td>
                </tr>
                
                <!-- APARTAT E -->
                <tr class="section-title">
                    <td class="col-apartat">E<br>MATERIALS</td>
                    <td>Estructura</td>
                    <td>
                        <div class="option-line">
                            <div class="compact-options">
                                <div class="checkbox-group">
                                    <input type="checkbox" id="e1_1" class="option-checkbox">
                                    <label for="e1_1" class="option-label">Fusta</label>
                                    <span class="punt-value">(5)</span>
                                </div>
                                <div class="checkbox-group">
                                    <input type="checkbox" id="e1_2" class="option-checkbox">
                                    <label for="e1_2" class="option-label">Bigues visibles</label>
                                    <span class="punt-value">(1)</span>
                                </div>
                                <div class="checkbox-group">
                                    <input type="checkbox" id="e1_3" class="option-checkbox">
                                    <label for="e1_3" class="option-label">Obra</label>
                                    <span class="punt-value">(0)</span>
                                </div>
                            </div>
                        </div>
                    </td>
                    <td>
                        <input type="text" class="score-input" id="puntuacio_e1" value="0" readonly="">
                    </td>
                </tr>
                <tr>
                    <td></td>
                    <td>Coberta</td>
                    <td>
                        <div class="option-line">
                            <div class="compact-options">
                                <div class="checkbox-group">
                                    <input type="checkbox" id="e2_1" class="option-checkbox">
                                    <label for="e2_1" class="option-label">Vegetal (Veg.)</label>
                                    <span class="punt-value">(3)</span>
                                </div>
                                <div class="checkbox-group">
                                    <input type="checkbox" id="e2_2" class="option-checkbox">
                                    <label for="e2_2" class="option-label">Tela asfàltica</label>
                                    <span class="punt-value">(2)</span>
                                </div>
                                <div class="checkbox-group">
                                    <input type="checkbox" id="e2_3" class="option-checkbox">
                                    <label for="e2_3" class="option-label">Teula/fibrociment</label>
                                    <span class="punt-value">(0)</span>
                                </div>
                            </div>
                        </div>
                    </td>
                    <td>
                        <input type="text" class="score-input" id="puntuacio_e2" value="0" readonly="">
                    </td>
                </tr>
                <tr>
                    <td></td>
                    <td>Canals</td>
                    <td>
                        <div class="option-line">
                            <div class="compact-options">
                                <div class="checkbox-group">
                                    <input type="checkbox" id="e3_1" class="option-checkbox">
                                    <label for="e3_1" class="option-label">Vegetal mort (Veg.)</label>
                                    <span class="punt-value">(3)</span>
                                </div>
                                <div class="checkbox-group">
                                    <input type="checkbox" id="e3_2" class="option-checkbox">
                                    <label for="e3_2" class="option-label">PVC</label>
                                    <span class="punt-value">(2)</span>
                                </div>
                                <div class="checkbox-group">
                                    <input type="checkbox" id="e3_3" class="option-checkbox">
                                    <label for="e3_3" class="option-label">Metall/fibrociment</label>
                                    <span class="punt-value">(0)</span>
                                </div>
                            </div>
                        </div>
                    </td>
                    <td>
                        <input type="text" class="score-input" id="puntuacio_e3" value="0" readonly="">
                    </td>
                </tr>
                <tr>
                    <td></td>
                    <td>Finestres</td>
                    <td>
                        <div class="option-line">
                            <div class="compact-options">
                                <div class="checkbox-group">
                                    <input type="checkbox" id="e4_1" class="option-checkbox">
                                    <label for="e4_1" class="option-label">PVC</label>
                                    <span class="punt-value">(3)</span>
                                </div>
                                <div class="checkbox-group">
                                    <input type="checkbox" id="e4_2" class="option-checkbox">
                                    <label for="e4_2" class="option-label">Fusta</label>
                                    <span class="punt-value">(2)</span>
                                </div>
                                <div class="checkbox-group">
                                    <input type="checkbox" id="e4_3" class="option-checkbox">
                                    <label for="e4_3" class="option-label">Metall (Alum./Acer)</label>
                                    <span class="punt-value">(0)</span>
                                </div>
                            </div>
                        </div>
                    </td>
                    <td>
                        <input type="text" class="score-input" id="puntuacio_e4" value="0" readonly="">
                    </td>
                </tr>
                <tr>
                    <td></td>
                    <td>Persianes</td>
                    <td>
                        <div class="option-line">
                            <div class="compact-options">
                                <div class="checkbox-group">
                                    <input type="checkbox" id="e5_1" class="option-checkbox">
                                    <label for="e5_1" class="option-label">Cap</label>
                                    <span class="punt-value">(5)</span>
                                </div>
                                <div class="checkbox-group">
                                    <input type="checkbox" id="e5_2" class="option-checkbox">
                                    <label for="e5_2" class="option-label">PVC</label>
                                    <span class="punt-value">(4)</span>
                                </div>
                                <div class="checkbox-group">
                                    <input type="checkbox" id="e5_3" class="option-checkbox">
                                    <label for="e5_3" class="option-label">Fusta massissa (&gt;2cm)</label>
                                    <span class="punt-value">(1)</span>
                                </div>
                            </div>
                        </div>
                    </td>
                    <td>
                        <input type="text" class="score-input" id="puntuacio_e5" value="0" readonly="">
                    </td>
                </tr>
                <tr>
                    <td></td>
                    <td>Xemeneia</td>
                    <td>
                        <div class="option-line">
                            <div class="compact-options">
                                <div class="checkbox-group">
                                    <input type="checkbox" id="e6_1" class="option-checkbox">
                                    <label for="e6_1" class="option-label">Lliure</label>
                                    <span class="punt-value">(3)</span>
                                </div>
                                <div class="checkbox-group">
                                    <input type="checkbox" id="e6_2" class="option-checkbox">
                                    <label for="e6_2" class="option-label">Protegida (reixa)</label>
                                    <span class="punt-value">(1)</span>
                                </div>
                            </div>
                        </div>
                    </td>
                    <td>
                        <input type="text" class="score-input" id="puntuacio_e6" value="0" readonly="">
                    </td>
                </tr>
                <tr class="subtotal-row">
                    <td colspan="3">SUBTOTAL APARTAT E →</td>
                    <td><input type="text" class="score-input" id="subtotal_e" value="0" readonly=""></td>
                </tr>
            </tbody>
        </table>
        
        <!-- SÍNTESI I INTERPRETACIÓ COMPACTA -->
        <div class="synthesis-section">
            <div class="synthesis-title">SÍNTESI I INTERPRETACIÓ DEL RISC</div>
            
            <div class="synthesis-grid">
                <div class="synthesis-item">
                    <div class="synthesis-label">PUNTS A</div>
                    <input type="text" class="score-input" id="total_a" value="0" readonly="">
                </div>
                <div class="synthesis-item">
                    <div class="synthesis-label">PUNTS B</div>
                    <input type="text" class="score-input" id="total_b" value="0" readonly="">
                </div>
                <div class="synthesis-item">
                    <div class="synthesis-label">PUNTS C</div>
                    <input type="text" class="score-input" id="total_c" value="0" readonly="">
                </div>
                <div class="synthesis-item">
                    <div class="synthesis-label">PUNTS D</div>
                    <input type="text" class="score-input" id="total_d" value="0" readonly="">
                </div>
                <div class="synthesis-item">
                    <div class="synthesis-label">PUNTS E</div>
                    <input type="text" class="score-input" id="total_e" value="0" readonly="">
                </div>
                
                <div class="total-box">
                    <span class="total-label">TOTAL PUNTUACIÓ:</span>
                    <input type="text" class="score-input" id="total_general" value="0" readonly="">
                </div>
            </div>
            
            <div class="interpretation">
                <div class="interpretation-title">INTERPRETACIÓ DEL RISC:</div>
                <div class="interpretation-grid">
                    <div class="interpretation-item">
                        <input type="checkbox" id="risk_low" class="interpretation-checkbox" disabled="">
                        <label for="risk_low" class="option-label risk-low">0-15 punts: ✓ (Risc baix)</label>
                    </div>
                    <div class="interpretation-item">
                        <input type="checkbox" id="risk_moderate" class="interpretation-checkbox" disabled="">
                        <label for="risk_moderate" class="option-label risk-moderate">16-31 punts: △ (Risc moderat)</label>
                    </div>
                    <div class="interpretation-item">
                        <input type="checkbox" id="risk_high" class="interpretation-checkbox" disabled="">
                        <label for="risk_high" class="option-label risk-high">32-46 punts: (Risc alt)</label>
                    </div>
                    <div class="interpretation-item">
                        <input type="checkbox" id="risk_extreme" class="interpretation-checkbox" disabled="">
                        <label for="risk_extreme" class="option-label risk-extreme">≥47 punts: (Risc molt alt / extrem)</label>
                    </div>
                </div>
            </div>
            
            <div class="note">
                <strong>Nota:</strong> Aquest qüestionari permet una avaluació ràpida del risc. Per a una anàlisi completa, consulti amb tècnics especialitzats en prevenció d'incendis forestals.
            </div>
        </div>
    </div>
    
    <!-- Controls no imprimibles -->
    <div class="controls no-print">
        <button onclick="calcularPuntuacions()">Calcular</button>
        <button onclick="window.print()">Imprimir/PDF</button>
        <button onclick="resetForm()">Netejar</button>
    </div>

    <script>
        // Objecte amb les puntuacions per cada opció
        const puntuacions = {
            // Apartat A
            'a1_1': 4, 'a1_2': 2, 'a1_3': 0,
            'a2_1': 2, 'a2_2': 1, 'a2_3': 0,
            
            // Apartat B
            'b1_1': 4, 'b1_2': 3, 'b1_3': 2, 'b1_4': 1, 'b1_5': 0,
            'b2_1': 3, 'b2_2': 2, 'b2_3': 1, 'b2_4': 0,
            'b3_1': 3, 'b3_2': 1, 'b3_3': 0,
            
            // Apartat C
            'c1_1': 3, 'c1_2': 2, 'c1_3': 1, 'c1_4': 0,
            'c2_1': 2, 'c2_2': 1, 'c2_3': 0, 'c2_4': 2, 'c2_5': 3,
            'c3_1': 0, 'c3_2': 4, 'c3_3': 3, 'c3_4': 2,
            'c4_1': 3, 'c4_2': 2, 'c4_3': 0,
            
            // Apartat D
            'd1_1': 2, 'd1_2': 0,
            'd2_1': 3, 'd2_2': 5, 'd2_3': 0,
            'd3_1': 2, 'd3_2': 1, 'd3_3': 0,
            
            // Apartat E
            'e1_1': 5, 'e1_2': 1, 'e1_3': 0,
            'e2_1': 3, 'e2_2': 2, 'e2_3': 0,
            'e3_1': 3, 'e3_2': 2, 'e3_3': 0,
            'e4_1': 3, 'e4_2': 2, 'e4_3': 0,
            'e5_1': 5, 'e5_2': 4, 'e5_3': 1,
            'e6_1': 3, 'e6_2': 1
        };
        
        // Grups exclusius (comportament de botó d'opció)
        const grupsExclusius = {
            'a1': ['a1_1', 'a1_2', 'a1_3'],
            'a2': ['a2_1', 'a2_2', 'a2_3'],
            'b1': ['b1_1', 'b1_2', 'b1_3', 'b1_4', 'b1_5'],
            'b2': ['b2_1', 'b2_2', 'b2_3', 'b2_4'],
            'b3': ['b3_1', 'b3_2', 'b3_3'],
            'c1': ['c1_1', 'c1_2', 'c1_3', 'c1_4'],
            'c2_mat': ['c2_1', 'c2_2', 'c2_3'],
            'c3': ['c3_1', 'c3_2', 'c3_3', 'c3_4'],
            'c4': ['c4_1', 'c4_2', 'c4_3'],
            'd1': ['d1_1', 'd1_2'],
            'd2': ['d2_1', 'd2_2', 'd2_3'],
            'd3': ['d3_1', 'd3_2', 'd3_3'],
            'e1': ['e1_1', 'e1_2', 'e1_3'],
            'e2': ['e2_1', 'e2_2', 'e2_3'],
            'e3': ['e3_1', 'e3_2', 'e3_3'],
            'e4': ['e4_1', 'e4_2', 'e4_3'],
            'e5': ['e5_1', 'e5_2', 'e5_3'],
            'e6': ['e6_1', 'e6_2']
        };
        
        // Configurar comportament de grups exclusius
        function configurarGrupsExclusius() {
            for (const grup in grupsExclusius) {
                const ids = grupsExclusius[grup];
                ids.forEach(id => {
                    const checkbox = document.getElementById(id);
                    if (checkbox) {
                        checkbox.addEventListener('change', function() {
                            if (this.checked) {
                                // Desmarcar altres checkboxes del mateix grup
                                ids.forEach(otherId => {
                                    if (otherId !== id) {
                                        const otherCheckbox = document.getElementById(otherId);
                                        if (otherCheckbox) otherCheckbox.checked = false;
                                    }
                                });
                            }
                            calcularPuntuacions();
                        });
                    }
                });
            }
            
            // Checkboxes que NO són exclusius (es poden marcar múltiples)
            const checkboxesMultiples = ['c2_4', 'c2_5'];
            checkboxesMultiples.forEach(id => {
                const checkbox = document.getElementById(id);
                if (checkbox) {
                    checkbox.addEventListener('change', calcularPuntuacions);
                }
            });
        }
        
        // Funció per calcular totes les puntuacions
        function calcularPuntuacions() {
            // Inicialitzar totals
            let totalA = 0, totalB = 0, totalC = 0, totalD = 0, totalE = 0;
            
            // Calcular cada apartat
            totalA = calcularGrup(['a1_1', 'a1_2', 'a1_3']) + calcularGrup(['a2_1', 'a2_2', 'a2_3']);
            totalB = calcularGrup(['b1_1', 'b1_2', 'b1_3', 'b1_4', 'b1_5']) +
                     calcularGrup(['b2_1', 'b2_2', 'b2_3', 'b2_4']) +
                     calcularGrup(['b3_1', 'b3_2', 'b3_3']);
            totalC = calcularGrup(['c1_1', 'c1_2', 'c1_3', 'c1_4']) +
                     (calcularGrup(['c2_1', 'c2_2', 'c2_3']) + 
                      (document.getElementById('c2_4').checked ? 2 : 0) +
                      (document.getElementById('c2_5').checked ? 3 : 0)) +
                     calcularGrup(['c3_1', 'c3_2', 'c3_3', 'c3_4']) +
                     calcularGrup(['c4_1', 'c4_2', 'c4_3']);
            totalD = calcularGrup(['d1_1', 'd1_2']) +
                     calcularGrup(['d2_1', 'd2_2', 'd2_3']) +
                     calcularGrup(['d3_1', 'd3_2', 'd3_3']);
            totalE = calcularGrup(['e1_1', 'e1_2', 'e1_3']) +
                     calcularGrup(['e2_1', 'e2_2', 'e2_3']) +
                     calcularGrup(['e3_1', 'e3_2', 'e3_3']) +
                     calcularGrup(['e4_1', 'e4_2', 'e4_3']) +
                     calcularGrup(['e5_1', 'e5_2', 'e5_3']) +
                     calcularGrup(['e6_1', 'e6_2']);
            
            // Actualitzar puntuacions per ítem
            document.getElementById('puntuacio_a1').value = calcularGrup(['a1_1', 'a1_2', 'a1_3']);
            document.getElementById('puntuacio_a2').value = calcularGrup(['a2_1', 'a2_2', 'a2_3']);
            document.getElementById('puntuacio_b1').value = calcularGrup(['b1_1', 'b1_2', 'b1_3', 'b1_4', 'b1_5']);
            document.getElementById('puntuacio_b2').value = calcularGrup(['b2_1', 'b2_2', 'b2_3', 'b2_4']);
            document.getElementById('puntuacio_b3').value = calcularGrup(['b3_1', 'b3_2', 'b3_3']);
            document.getElementById('puntuacio_c1').value = calcularGrup(['c1_1', 'c1_2', 'c1_3', 'c1_4']);
            document.getElementById('puntuacio_c2').value = calcularGrup(['c2_1', 'c2_2', 'c2_3']) +
                (document.getElementById('c2_4').checked ? 2 : 0) +
                (document.getElementById('c2_5').checked ? 3 : 0);
            document.getElementById('puntuacio_c3').value = calcularGrup(['c3_1', 'c3_2', 'c3_3', 'c3_4']);
            document.getElementById('puntuacio_c4').value = calcularGrup(['c4_1', 'c4_2', 'c4_3']);
            document.getElementById('puntuacio_d1').value = calcularGrup(['d1_1', 'd1_2']);
            document.getElementById('puntuacio_d2').value = calcularGrup(['d2_1', 'd2_2', 'd2_3']);
            document.getElementById('puntuacio_d3').value = calcularGrup(['d3_1', 'd3_2', 'd3_3']);
            document.getElementById('puntuacio_e1').value = calcularGrup(['e1_1', 'e1_2', 'e1_3']);
            document.getElementById('puntuacio_e2').value = calcularGrup(['e2_1', 'e2_2', 'e2_3']);
            document.getElementById('puntuacio_e3').value = calcularGrup(['e3_1', 'e3_2', 'e3_3']);
            document.getElementById('puntuacio_e4').value = calcularGrup(['e4_1', 'e4_2', 'e4_3']);
            document.getElementById('puntuacio_e5').value = calcularGrup(['e5_1', 'e5_2', 'e5_3']);
            document.getElementById('puntuacio_e6').value = calcularGrup(['e6_1', 'e6_2']);
            
            // Actualitzar subtotals
            document.getElementById('subtotal_a').value = totalA;
            document.getElementById('subtotal_b').value = totalB;
            document.getElementById('subtotal_c').value = totalC;
            document.getElementById('subtotal_d').value = totalD;
            document.getElementById('subtotal_e').value = totalE;
            
            // Actualitzar totals a síntesi
            document.getElementById('total_a').value = totalA;
            document.getElementById('total_b').value = totalB;
            document.getElementById('total_c').value = totalC;
            document.getElementById('total_d').value = totalD;
            document.getElementById('total_e').value = totalE;
            
            // Calcular i mostrar total general
            const totalGeneral = totalA + totalB + totalC + totalD + totalE;
            document.getElementById('total_general').value = totalGeneral;
            
            // Actualitzar interpretació
            actualitzarInterpretacio(totalGeneral);
        }
        
        // Funció auxiliar per calcular un grup
        function calcularGrup(ids) {
            let puntuacio = 0;
            ids.forEach(id => {
                const checkbox = document.getElementById(id);
                if (checkbox && checkbox.checked) {
                    puntuacio += puntuacions[id] || 0;
                }
            });
            return puntuacio;
        }
        
        // Funció per actualitzar la interpretació
        function actualitzarInterpretacio(total) {
            // Desmarcar totes les interpretacions
            document.getElementById('risk_low').checked = false;
            document.getElementById('risk_moderate').checked = false;
            document.getElementById('risk_high').checked = false;
            document.getElementById('risk_extreme').checked = false;
            
            // Marcar la interpretació corresponent
            if (total <= 15) {
                document.getElementById('risk_low').checked = true;
            } else if (total <= 31) {
                document.getElementById('risk_moderate').checked = true;
            } else if (total <= 46) {
                document.getElementById('risk_high').checked = true;
            } else {
                document.getElementById('risk_extreme').checked = true;
            }
        }
        
        // Funció per netejar el formulari
        function resetForm() {
            if (confirm('Vols netejar tot el formulari?')) {
                // Netejar tots els checkboxes
                const checkboxes = document.querySelectorAll('input[type="checkbox"]');
                checkboxes.forEach(checkbox => {
                    checkbox.checked = false;
                });
                
                // Netejar tots els camps de text
                const textInputs = document.querySelectorAll('input[type="text"]');
                textInputs.forEach(input => {
                    if (input.id.startsWith('puntuacio_') || 
                        input.id.startsWith('subtotal_') || 
                        input.id.startsWith('total_') ||
                        input.id === 'total_general') {
                        input.value = '0';
                    } else {
                        input.value = '';
                    }
                });
                
                // Reiniciar interpretació
                actualitzarInterpretacio(0);
            }
        }
        
        // Inicialització
        document.addEventListener('DOMContentLoaded', function() {
            configurarGrupsExclusius();
            calcularPuntuacions();
            
            // Afegir event listeners a tots els checkboxes
            const checkboxes = document.querySelectorAll('.option-checkbox');
            checkboxes.forEach(checkbox => {
                checkbox.addEventListener('change', calcularPuntuacions);
            });
        });
    </script>

</body></html>
