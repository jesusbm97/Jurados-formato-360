<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, user-scalable=no">
    <title>Formato 360 - Tauro Esencia</title>
    <meta name="theme-color" content="#8B0000">
    <link rel="manifest" href="data:application/json;base64,eyJuYW1lIjoiRm9ybWF0byAzNjAiLCJzaG9ydF9uYW1lIjoiRjM2MCIsImRlc2NyaXB0aW9uIjoiU2lzdGVtYSBkZSBjb25jdXJzb3MgZGUgcmVjb3J0ZXMiLCJzdGFydF91cmwiOiIuIiwiZGlzcGxheSI6InN0YW5kYWxvbmUiLCJiYWNrZ3JvdW5kX2NvbG9yIjoiI2ZmZmZmZiIsInRoZW1lX2NvbG9yIjoiIzhCMDAwMCIsImljb25zIjpbeyJzcmMiOiJkYXRhOmltYWdlL3N2Zyt4bWw7YmFzZTY0LFBITjJaeUI0Yld4dWN6MGlhSFIwY0RvdkwzZDNkeTUzTXk1dmNtY3ZNakF3TUM5emRtY2lJSEJ5WlhObGNuWmxRWE5wZW1VOUlDSXZjbWwyWlNBOUlDSWlPaUpDWVdGa2JXbHVJbjA9Iiwic2l6ZXMiOiIxOTJ4MTkyIiwidHlwZSI6ImltYWdlL3N2Zyt4bWwifSx7InNyYyI6ImRhdGE6aW1hZ2Uvc3ZnK3htbDtiYXNlNjQsUEhOMlp5QjRiV3h1Y3owaWFIUjBjRG92TDNkM2R5NTNNeTV2Y21jd01qQXdNQzl6ZG1jaUlIQnlaWE5sY25abFFYTnBlbVU5SUNJdmNtTDJZM1Z5WDJsa0lDSmRMQ0pqY21Wa2FYWW9JbkJ2Ym1VaUlIZHBaSFJvUFNJeE1qQXhOREl4TVRJd01UZ3hNakUzTVNJc0ltTnZaR1V1WTI5dExtTnZiUzhpUGp4MFpYaDBiR1VpT2lKQ1lXWmhiV2xzZVRvZ2MzUnliMnRsTFhkcFpIUm9QU0l4TWpBeE5USXhNVEl3TVRreE1qRTNNU0lzSW1OdmRXNWtJbjBpWlhoaGJYQnNaUzVqYjIwaUx6ND0iLCJzaXplcyI6IjUxMng1MTIiLCJ0eXBlIjoiaW1hZ2Uvc3ZnK3htbCJ9XX0=">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, sans-serif;
        }
        
        body {
            background: linear-gradient(135deg, #8B0000, #a52a2a);
            color: #333;
            min-height: 100vh;
            overflow-x: hidden;
        }
        
        .app {
            max-width: 100%;
            margin: 0 auto;
            background: white;
            min-height: 100vh;
            position: relative;
        }
        
        .header {
            background: #8B0000;
            color: white;
            padding: 15px;
            text-align: center;
            position: sticky;
            top: 0;
            z-index: 100;
            box-shadow: 0 2px 10px rgba(0,0,0,0.2);
        }
        
        .header h1 {
            font-size: 1.8rem;
            margin-bottom: 5px;
        }
        
        .header p {
            font-size: 0.9rem;
            opacity: 0.9;
        }
        
        .content {
            padding: 15px;
            padding-bottom: 80px;
        }
        
        .screen {
            display: none;
        }
        
        .screen.active {
            display: block;
        }
        
        .card {
            background: white;
            border-radius: 10px;
            padding: 15px;
            margin-bottom: 15px;
            box-shadow: 0 2px 10px rgba(0,0,0,0.1);
        }
        
        .card h3 {
            color: #8B0000;
            margin-bottom: 15px;
            font-size: 1.2rem;
        }
        
        .form-group {
            margin-bottom: 15px;
        }
        
        label {
            display: block;
            margin-bottom: 5px;
            font-weight: bold;
            color: #555;
            font-size: 0.9rem;
        }
        
        input, select, textarea {
            width: 100%;
            padding: 12px;
            border: 1px solid #ddd;
            border-radius: 8px;
            font-size: 1rem;
            box-sizing: border-box;
        }
        
        button {
            background: #8B0000;
            color: white;
            border: none;
            padding: 12px 20px;
            border-radius: 8px;
            cursor: pointer;
            font-size: 1rem;
            font-weight: bold;
            width: 100%;
            margin-top: 10px;
            transition: all 0.3s;
        }
        
        button:hover {
            background: #a52a2a;
        }
        
        .btn-secondary {
            background: #6c757d;
        }
        
        .btn-secondary:hover {
            background: #5a6268;
        }
        
        .btn-success {
            background: #28a745;
        }
        
        .btn-success:hover {
            background: #218838;
        }
        
        .btn-warning {
            background: #ffc107;
            color: #333;
        }
        
        .btn-warning:hover {
            background: #e0a800;
        }
        
        .jurado-card {
            background: #f8f9fa;
            border: 1px solid #ddd;
            border-radius: 10px;
            padding: 12px;
            margin-bottom: 10px;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }
        
        .jurado-name {
            font-weight: bold;
        }
        
        .jurado-code {
            background: #8B0000;
            color: white;
            padding: 5px 10px;
            border-radius: 5px;
            font-family: monospace;
            font-weight: bold;
            font-size: 0.9rem;
        }
        
        .toro-orden {
            background: #f8f9fa;
            border: 1px solid #ddd;
            border-radius: 10px;
            padding: 12px;
            margin-bottom: 10px;
        }
        
        .toro-orden h4 {
            color: #8B0000;
            margin-bottom: 8px;
        }
        
        .orden-list {
            display: flex;
            flex-wrap: wrap;
            gap: 8px;
        }
        
        .orden-item {
            background: white;
            border: 1px solid #ddd;
            border-radius: 5px;
            padding: 6px 10px;
            font-size: 0.85rem;
            font-weight: bold;
        }
        
        .puntuacion-table {
            width: 100%;
            border-collapse: collapse;
            margin: 15px 0;
            font-size: 0.9rem;
        }
        
        .puntuacion-table th, .puntuacion-table td {
            padding: 10px 8px;
            text-align: left;
            border-bottom: 1px solid #ddd;
        }
        
        .puntuacion-table th {
            background-color: #8B0000;
            color: white;
            font-size: 0.85rem;
        }
        
        .puntuacion-table input {
            width: 60px;
            text-align: center;
            padding: 8px;
        }
        
        .clasificacion-table {
            width: 100%;
            border-collapse: collapse;
            margin: 15px 0;
            font-size: 0.9rem;
        }
        
        .clasificacion-table th, .clasificacion-table td {
            padding: 10px 8px;
            text-align: left;
            border-bottom: 1px solid #ddd;
        }
        
        .clasificacion-table th {
            background-color: #8B0000;
            color: white;
            font-size: 0.85rem;
        }
        
        .clasificacion-table tr:nth-child(even) {
            background-color: #f8f9fa;
        }
        
        .finalista {
            background-color: #e8f5e9 !important;
            font-weight: bold;
        }
        
        .finalistas-list {
            margin: 15px 0;
        }
        
        .finalista-item {
            background: #f8f9fa;
            border: 1px solid #ddd;
            border-radius: 10px;
            padding: 12px;
            margin-bottom: 10px;
            display: flex;
            align-items: center;
        }
        
        .finalista-position {
            background: #8B0000;
            color: white;
            width: 30px;
            height: 30px;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            font-weight: bold;
            margin-right: 15px;
            flex-shrink: 0;
        }
        
        .rondas-container {
            margin: 15px 0;
        }
        
        .ronda-input {
            margin-bottom: 15px;
        }
        
        .ronda-input label {
            font-weight: bold;
            margin-bottom: 8px;
            display: block;
        }
        
        .ronda-input .inputs-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(80px, 1fr));
            gap: 10px;
        }
        
        .ronda-input .input-group {
            display: flex;
            flex-direction: column;
            align-items: center;
        }
        
        .ronda-input .input-group label {
            font-size: 0.8rem;
            margin-bottom: 5px;
            text-align: center;
        }
        
        .ronda-input .input-group input {
            width: 100%;
            padding: 8px;
            text-align: center;
        }
        
        .resultado-final {
            background: #e8f5e9;
            border-radius: 10px;
            padding: 20px;
            margin-top: 20px;
            text-align: center;
        }
        
        .resultado-final h3 {
            color: #2e7d32;
            font-size: 1.5rem;
            margin-bottom: 15px;
        }
        
        .ganador {
            font-size: 1.3rem;
            font-weight: bold;
            color: #2e7d32;
            margin-bottom: 10px;
        }
        
        .notification {
            position: fixed;
            top: 20px;
            left: 50%;
            transform: translateX(-50%);
            background: #4CAF50;
            color: white;
            padding: 12px 20px;
            border-radius: 8px;
            box-shadow: 0 4px 8px rgba(0,0,0,0.2);
            z-index: 1000;
            font-weight: bold;
            max-width: 90%;
            text-align: center;
        }
        
        .notification.error {
            background: #f44336;
        }
        
        .install-banner {
            background: #8B0000;
            color: white;
            text-align: center;
            padding: 10px;
            position: sticky;
            bottom: 0;
            z-index: 100;
            font-size: 0.9rem;
        }
        
        .install-banner button {
            background: white;
            color: #8B0000;
            padding: 5px 15px;
            border-radius: 5px;
            font-size: 0.9rem;
            width: auto;
            margin: 5px;
        }
        
        .login-form {
            background: white;
            border-radius: 10px;
            padding: 20px;
            margin: 20px;
            box-shadow: 0 4px 15px rgba(0,0,0,0.1);
            max-width: 400px;
            margin-left: auto;
            margin-right: auto;
        }
        
        .login-form h2 {
            color: #8B0000;
            margin-bottom: 20px;
            text-align: center;
        }
        
        .participantes-list {
            margin: 15px 0;
        }
        
        .participante-item {
            display: flex;
            align-items: center;
            margin-bottom: 10px;
        }
        
        .participante-number {
            background: #8B0000;
            color: white;
            width: 30px;
            height: 30px;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            font-weight: bold;
            margin-right: 15px;
            flex-shrink: 0;
        }
        
        .participante-name {
            flex: 1;
        }
        
        .simular-btn {
            background: #28a745;
            margin-top: 10px;
        }
        
        .simular-btn:hover {
            background: #218838;
        }
        
        .debug-panel {
            background: #f8f9fa;
            border: 1px solid #ddd;
            border-radius: 10px;
            padding: 15px;
            margin: 15px 0;
        }
        
        .debug-panel h4 {
            color: #8B0000;
            margin-bottom: 10px;
        }
        
        .debug-info {
            font-size: 0.85rem;
            color: #666;
            margin-bottom: 5px;
        }
        
        .access-options {
            display: flex;
            flex-direction: column;
            gap: 20px;
            margin: 20px;
        }
        
        .access-card {
            background: white;
            border-radius: 15px;
            padding: 30px;
            text-align: center;
            box-shadow: 0 5px 20px rgba(0,0,0,0.1);
            transition: transform 0.3s;
        }
        
        .access-card:hover {
            transform: translateY(-5px);
        }
        
        .access-card h3 {
            color: #8B0000;
            margin-bottom: 15px;
            font-size: 1.5rem;
        }
        
        .access-card p {
            margin-bottom: 20px;
            color: #666;
        }
        
        .access-icon {
            font-size: 3rem;
            margin-bottom: 15px;
        }
        
        .btn-access {
            background: #8B0000;
            color: white;
            border: none;
            padding: 15px 30px;
            border-radius: 8px;
            cursor: pointer;
            font-size: 1.1rem;
            font-weight: bold;
            width: auto;
            transition: all 0.3s;
        }
        
        .btn-access:hover {
            background: #a52a2a;
        }
        
        .btn-jurado {
            background: #28a745;
        }
        
        .btn-jurado:hover {
            background: #218838;
        }
        
        .back-btn {
            background: #6c757d;
            color: white;
            border: none;
            padding: 8px 15px;
            border-radius: 5px;
            cursor: pointer;
            font-size: 0.9rem;
            width: auto;
            margin-right: 10px;
        }
        
        .back-btn:hover {
            background: #5a6268;
        }
        
        .header-actions {
            position: absolute;
            right: 15px;
            top: 15px;
            display: flex;
            align-items: center;
        }
        
        .auto-update {
            background: #e8f5e9;
            border: 1px solid #c8e6c9;
            border-radius: 8px;
            padding: 10px;
            margin: 15px 0;
            display: flex;
            align-items: center;
        }
        
        .auto-update-icon {
            color: #4caf50;
            margin-right: 10px;
            font-size: 1.2rem;
        }
        
        .auto-update-text {
            color: #2e7d32;
            font-weight: bold;
        }
        
        .puntuacion-summary {
            background: #f8f9fa;
            border: 1px solid #ddd;
            border-radius: 8px;
            padding: 10px;
            margin-top: 10px;
            font-size: 0.85rem;
            color: #666;
        }
        
        .final-puntuacion-table {
            width: 100%;
            border-collapse: collapse;
            margin: 15px 0;
            font-size: 0.9rem;
        }
        
        .final-puntuacion-table th, .final-puntuacion-table td {
            padding: 10px 8px;
            text-align: center;
            border-bottom: 1px solid #ddd;
        }
        
        .final-puntuacion-table th {
            background-color: #8B0000;
            color: white;
            font-size: 0.85rem;
        }
        
        .final-puntuacion-table input {
            width: 60px;
            text-align: center;
            padding: 8px;
        }
        
        .final-ready {
            background: #e3f2fd;
            border: 1px solid #bbdefb;
            border-radius: 8px;
            padding: 15px;
            margin: 15px 0;
            text-align: center;
        }
        
        .final-ready h4 {
            color: #1976d2;
            margin-bottom: 10px;
        }
        
        .final-ready p {
            color: #1976d2;
            font-weight: bold;
        }
        
        .final-results-table {
            width: 100%;
            border-collapse: collapse;
            margin: 15px 0;
            font-size: 0.9rem;
        }
        
        .final-results-table th, .final-results-table td {
            padding: 12px 8px;
            text-align: left;
            border-bottom: 1px solid #ddd;
        }
        
        .final-results-table th {
            background-color: #8B0000;
            color: white;
            font-size: 0.85rem;
        }
        
        .final-results-table .posicion-final {
            font-weight: bold;
            font-size: 1.1rem;
            color: #8B0000;
        }
        
        .final-results-table .ganador-final {
            background-color: #e8f5e9;
            font-weight: bold;
            font-size: 1.1rem;
        }
        
        .posiciones-toros {
            background: #f8f9fa;
            border: 1px solid #ddd;
            border-radius: 10px;
            padding: 15px;
            margin: 15px 0;
        }
        
        .posiciones-toros h4 {
            color: #8B0000;
            margin-bottom: 15px;
            text-align: center;
        }
        
        .posiciones-toros-table {
            width: 100%;
            border-collapse: collapse;
            font-size: 0.85rem;
        }
        
        .posiciones-toros-table th, .posiciones-toros-table td {
            padding: 8px 5px;
            text-align: center;
            border: 1px solid #ddd;
        }
        
        .posiciones-toros-table th {
            background-color: #8B0000;
            color: white;
        }
        
        .posiciones-toros-table .participante-nombre {
            font-weight: bold;
            text-align: left;
        }
        
        .eventos-lista {
            margin-top: 20px;
        }
        
        .evento-card {
            background: #f8f9fa;
            border: 1px solid #ddd;
            border-radius: 10px;
            padding: 15px;
            margin-bottom: 15px;
            box-shadow: 0 2px 5px rgba(0,0,0,0.1);
        }
        
        .evento-card h4 {
            color: #8B0000;
            margin-bottom: 10px;
        }
        
        .evento-card p {
            margin-bottom: 5px;
            color: #666;
        }
        
        .evento-actions {
            display: flex;
            gap: 10px;
            margin-top: 15px;
        }
        
        .btn-small {
            padding: 8px 15px;
            font-size: 0.9rem;
            width: auto;
        }
        
        .finalista-empate {
            background: #fff3cd;
            border: 1px solid #ffeaa7;
            border-radius: 8px;
            padding: 10px;
            margin: 10px 0;
        }
        
        .finalista-empate h4 {
            color: #856404;
            margin-bottom: 10px;
        }
        
        .import-export {
            display: flex;
            gap: 10px;
            margin-top: 10px;
        }
        
        .empate-selector {
            margin: 15px 0;
            padding: 15px;
            background: #fff3cd;
            border-radius: 8px;
            border: 1px solid #ffeaa7;
        }
        
        .empate-selector h4 {
            color: #856404;
            margin-bottom: 10px;
        }
        
        .empate-options {
            display: flex;
            flex-wrap: wrap;
            gap: 10px;
            margin-top: 10px;
        }
        
        .empate-option {
            background: white;
            border: 1px solid #ddd;
            border-radius: 5px;
            padding: 8px 12px;
            cursor: pointer;
            transition: all 0.2s;
        }
        
        .empate-option:hover {
            background: #f8f9fa;
        }
        
        .empate-option.selected {
            background: #8B0000;
            color: white;
        }
        
        .jurado-info {
            background: #e3f2fd;
            border: 1px solid #bbdefb;
            border-radius: 8px;
            padding: 10px;
            margin: 10px 0;
            text-align: center;
        }
        
        .jurado-info h4 {
            color: #1976d2;
            margin-bottom: 5px;
        }
        
        .jurado-info p {
            color: #1976d2;
            font-weight: bold;
        }
        
        .evento-estado {
            display: inline-block;
            padding: 3px 8px;
            border-radius: 4px;
            font-size: 0.8rem;
            font-weight: bold;
            margin-left: 10px;
        }
        
        .estado-activo {
            background: #e8f5e9;
            color: #2e7d32;
        }
        
        .estado-final {
            background: #e3f2fd;
            color: #1976d2;
        }
        
        .estado-completado {
            background: #fff3e0;
            color: #e65100;
        }
        
        .jurado-codigo-input {
            display: flex;
            gap: 10px;
            margin-top: 10px;
        }
        
        .jurado-codigo-input input {
            flex: 1;
        }
        
        .jurado-codigo-input button {
            width: auto;
            padding: 12px 20px;
            margin-top: 0;
        }
        
        .modal {
            display: none;
            position: fixed;
            z-index: 1000;
            left: 0;
            top: 0;
            width: 100%;
            height: 100%;
            background-color: rgba(0,0,0,0.5);
        }
        
        .modal-content {
            background-color: white;
            margin: 15% auto;
            padding: 20px;
            border-radius: 10px;
            width: 80%;
            max-width: 500px;
        }
        
        .close {
            color: #aaa;
            float: right;
            font-size: 28px;
            font-weight: bold;
            cursor: pointer;
        }
        
        .close:hover {
            color: black;
        }
        
        @media (max-width: 480px) {
            .header h1 {
                font-size: 1.5rem;
            }
            
            .content {
                padding: 10px;
            }
            
            .orden-list {
                flex-direction: column;
            }
            
            .orden-item {
                width: 100%;
            }
            
            .puntuacion-table {
                font-size: 0.8rem;
            }
            
            .puntuacion-table th, .puntuacion-table td {
                padding: 8px 5px;
            }
            
            .ronda-input .inputs-grid {
                grid-template-columns: repeat(2, 1fr);
            }
            
            .access-options {
                margin: 10px;
            }
            
            .access-card {
                padding: 20px;
            }
            
            .final-puntuacion-table {
                font-size: 0.8rem;
            }
            
            .final-puntuacion-table th, .final-puntuacion-table td {
                padding: 6px 4px;
            }
            
            .posiciones-toros-table {
                font-size: 0.75rem;
            }
            
            .posiciones-toros-table th, .posiciones-toros-table td {
                padding: 5px 3px;
            }
            
            .evento-actions {
                flex-direction: column;
            }
            
            .import-export {
                flex-direction: column;
            }
            
            .jurado-codigo-input {
                flex-direction: column;
            }
            
            .jurado-codigo-input button {
                width: 100%;
                margin-top: 10px;
            }
        }
    </style>
</head>
<body>
    <div class="app">
        <!-- Pantalla de acceso inicial -->
        <div id="access-screen" class="screen active">
            <div class="header">
                <h1>FORMATO 360</h1>
                <p>Tauro Esencia S.L.</p>
            </div>
            
            <div class="access-options">
                <div class="access-card">
                    <div class="access-icon">👤</div>
                    <h3>Organizador</h3>
                    <p>Crear y gestionar eventos</p>
                    <button class="btn-access" onclick="showOrganizadorLogin()">Acceder</button>
                </div>
                
                <div class="access-card">
                    <div class="access-icon">⚖️</div>
                    <h3>Jurado</h3>
                    <p>Puntuar concursos</p>
                    <button class="btn-access btn-jurado" onclick="showJuradoAccess()">Acceder</button>
                </div>
            </div>
        </div>
        
        <!-- Pantalla de login para organizador -->
        <div id="organizador-login-screen" class="screen">
            <div class="header">
                <h1>FORMATO 360</h1>
                <p>Tauro Esencia S.L.</p>
                <div class="header-actions">
                    <button class="back-btn" onclick="showAccessScreen()">← Volver</button>
                </div>
            </div>
            
            <div class="login-form">
                <h2>Acceso Organizador</h2>
                <div class="form-group">
                    <label for="password">Contraseña</label>
                    <input type="password" id="password" placeholder="Ingresa la contraseña">
                </div>
                <button onclick="loginOrganizador()">Entrar</button>
            </div>
        </div>
        
        <!-- Pantalla principal (organizador) - Lista de eventos -->
        <div id="organizador-screen" class="screen">
            <div class="header">
                <h1>FORMATO 360</h1>
                <p>Tauro Esencia S.L.</p>
                <div class="header-actions">
                    <button class="back-btn" onclick="logout()">Salir</button>
                </div>
            </div>
            
            <div class="content">
                <div class="card">
                    <h3>Mis Eventos</h3>
                    <button onclick="showCrearEvento()">Crear Nuevo Evento</button>
                    <div id="eventos-lista" class="eventos-lista"></div>
                </div>
                
                <div class="card">
                    <h3>Sincronización</h3>
                    <div class="import-export">
                        <button onclick="exportarEventos()">Exportar Eventos</button>
                        <button onclick="importarEventos()">Importar Eventos</button>
                    </div>
                    <input type="file" id="import-file" style="display:none" onchange="handleImport(event)">
                </div>
                
                <!-- Panel de depuración -->
                <div class="debug-panel">
                    <h4>Panel de Depuración</h4>
                    <div class="debug-info">Eventos creados: <span id="debug-eventos">0</span></div>
                    <div class="debug-info">Jurados creados: <span id="debug-jurados">0</span></div>
                    <div class="debug-info">Puntuaciones guardadas: <span id="debug-puntuaciones">0</span></div>
                    <button class="btn-secondary" onclick="limpiarDatos()">Limpiar todos los datos</button>
                </div>
            </div>
        </div>
        
        <!-- Pantalla de creación de evento -->
        <div id="crear-evento-screen" class="screen">
            <div class="header">
                <h1>FORMATO 360</h1>
                <p>Tauro Esencia S.L.</p>
                <div class="header-actions">
                    <button class="back-btn" onclick="volverAEventos()">← Volver</button>
                </div>
            </div>
            
            <div class="content">
                <div class="card">
                    <h3>Crear Nuevo Evento</h3>
                    <div class="form-group">
                        <label for="evento-nombre">Nombre del Evento</label>
                        <input type="text" id="evento-nombre" placeholder="Ej: Concurso de Primavera">
                    </div>
                    
                    <div class="form-group">
                        <label for="evento-tipo">Tipo de Concurso</label>
                        <select id="evento-tipo" onchange="actualizarParticipantes()">
                            <option value="normal">Normal (3 toros)</option>
                            <option value="extra">Extra (4 toros)</option>
                        </select>
                    </div>
                    
                    <div class="form-group">
                        <label for="evento-participantes">Número de Participantes</label>
                        <select id="evento-participantes" onchange="actualizarParticipantes()">
                            <option value="9">9 participantes</option>
                            <option value="12">12 participantes</option>
                            <option value="16">16 participantes</option>
                        </select>
                    </div>
                    
                    <div class="form-group">
                        <label>Orden del Toro 1 (Asigna nombres a cada número)</label>
                        <div id="participantes-lista" class="participantes-list"></div>
                    </div>
                    
                    <button onclick="crearEvento()">Crear Evento</button>
                </div>
            </div>
        </div>
        
        <!-- Pantalla de gestión de evento -->
        <div id="evento-gestion-screen" class="screen">
            <div class="header">
                <h1>FORMATO 360</h1>
                <p>Tauro Esencia S.L.</p>
                <div class="header-actions">
                    <button class="back-btn" onclick="volverAEventos()">← Volver</button>
                </div>
            </div>
            
            <div class="content">
                <div class="card">
                    <h3 id="evento-titulo"></h3>
                    <div id="evento-detalles"></div>
                </div>
                
                <div class="card">
                    <h3>Órdenes de Toros</h3>
                    <div id="ordenes-toros-gestion"></div>
                </div>
                
                <div class="card">
                    <h3>Jurados</h3>
                    <div id="jurados-gestion"></div>
                    <button onclick="invitarJurados()">Invitar Jurados</button>
                </div>
                
                <div class="card">
                    <h3>Clasificación</h3>
                    <button onclick="verClasificacion()">Ver Clasificación</button>
                    <button id="generar-final-btn" onclick="mostrarGenerarFinal()" style="display:none">Generar Final</button>
                </div>
                
                <div class="card">
                    <h3>Resultados Finales</h3>
                    <button id="ver-resultados-btn" onclick="verResultadosFinales()" style="display:none">Ver Resultados</button>
                </div>
            </div>
        </div>
        
        <!-- Pantalla para generar final -->
        <div id="generar-final-screen" class="screen">
            <div class="header">
                <h1>FORMATO 360</h1>
                <p>Tauro Esencia S.L.</p>
                <div class="header-actions">
                    <button class="back-btn" onclick="volverAGestion()">← Volver</button>
                </div>
            </div>
            
            <div class="content">
                <div class="card">
                    <h3>Generar Final</h3>
                    <p>Selecciona los 4 finalistas. Puedes cambiar el 4º clasificado en caso de empate.</p>
                    <div id="finalistas-seleccion"></div>
                    <div id="empate-selector" class="empate-selector" style="display:none;">
                        <h4>Empate en 4º puesto:</h4>
                        <div id="empate-options" class="empate-options"></div>
                    </div>
                    <button onclick="confirmarFinal()">Confirmar Finalistas</button>
                </div>
            </div>
        </div>
        
        <!-- Pantalla de acceso para jurado -->
        <div id="jurado-access-screen" class="screen">
            <div class="header">
                <h1>FORMATO 360</h1>
                <p>Tauro Esencia S.L.</p>
                <div class="header-actions">
                    <button class="back-btn" onclick="showAccessScreen()">← Volver</button>
                </div>
            </div>
            
            <div class="login-form">
                <h2>Acceso de Jurado</h2>
                <div class="form-group">
                    <label for="codigo-acceso">Código de Acceso</label>
                    <input type="text" id="codigo-acceso" placeholder="Ingresa tu código">
                </div>
                <button onclick="accederJurado()">Entrar</button>
            </div>
        </div>
        
        <!-- Pantalla de puntuación para jurado -->
        <div id="jurado-screen" class="screen">
            <div class="header">
                <h1>FORMATO 360</h1>
                <p>Tauro Esencia S.L.</p>
                <div class="header-actions">
                    <button class="back-btn" onclick="logoutJurado()">Salir</button>
                </div>
            </div>
            
            <div class="content">
                <div class="jurado-info">
                    <h4>Jurado: <span id="jurado-nombre"></span></h4>
                    <p>Evento: <span id="jurado-evento"></span></p>
                </div>
                
                <div class="card">
                    <h3>Puntuar Toros</h3>
                    <div class="form-group">
                        <label for="toro-select">Selecciona el Toro</label>
                        <select id="toro-select" onchange="cargarToro()">
                            <option value="toro1">Toro 1</option>
                            <option value="toro2">Toro 2</option>
                            <option value="toro3">Toro 3</option>
                            <option value="toro4">Toro 4</option>
                        </select>
                    </div>
                    
                    <div id="puntuaciones-form"></div>
                    
                    <button onclick="guardarPuntuaciones()">Guardar Puntuaciones</button>
                </div>
            </div>
        </div>
        
        <!-- Pantalla de puntuación de final para jurado -->
        <div id="jurado-final-screen" class="screen">
            <div class="header">
                <h1>FORMATO 360</h1>
                <p>Tauro Esencia S.L.</p>
                <div class="header-actions">
                    <button class="back-btn" onclick="logoutJurado()">Salir</button>
                </div>
            </div>
            
            <div class="content">
                <div class="jurado-info">
                    <h4>Jurado: <span id="jurado-nombre-final"></span></h4>
                    <p>Evento: <span id="jurado-evento-final"></span></p>
                </div>
                
                <div class="card">
                    <h3>Puntuar Final</h3>
                    <p>Los 4 finalistas en orden de clasificación</p>
                    
                    <table class="final-puntuacion-table">
                        <thead>
                            <tr>
                                <th>Posición</th>
                                <th>Finalista</th>
                                <th>Ronda 1</th>
                                <th>Ronda 2</th>
                                <th>Ronda 3</th>
                                <th>Ronda 4</th>
                                <th>Ronda 5</th>
                                <th>Ronda 6</th>
                                <th>Ronda 7</th>
                            </tr>
                        </thead>
                        <tbody id="final-puntuaciones-tbody">
                            <!-- Se llenará dinámicamente -->
                        </tbody>
                    </table>
                    
                    <button onclick="guardarPuntuacionesFinalJurado()">Guardar Puntuaciones</button>
                </div>
            </div>
        </div>
        
        <!-- Sección Clasificación -->
        <div id="clasificacion-screen" class="screen">
            <div class="header">
                <h1>FORMATO 360</h1>
                <p>Tauro Esencia S.L.</p>
                <div class="header-actions">
                    <button class="back-btn" onclick="volverAGestion()">← Volver</button>
                </div>
            </div>
            
            <div class="content">
                <div class="auto-update">
                    <span class="auto-update-icon">✓</span>
                    <span class="auto-update-text">Clasificación actualizada automáticamente</span>
                </div>
                
                <div class="card">
                    <h3>Clasificación Acumulada</h3>
                    <div id="tabla-clasificacion"></div>
                </div>
            </div>
        </div>
        
        <!-- Sección Resultados Finales -->
        <div id="resultados-screen" class="screen">
            <div class="header">
                <h1>FORMATO 360</h1>
                <p>Tauro Esencia S.L.</p>
                <div class="header-actions">
                    <button class="back-btn" onclick="volverAGestion()">← Volver</button>
                </div>
            </div>
            
            <div class="content">
                <div class="card">
                    <h3>Resultados Finales del Concurso</h3>
                    <div id="tabla-resultados-finales"></div>
                </div>
            </div>
        </div>
        
        <!-- Modal para invitar jurados -->
        <div id="juradosModal" class="modal">
            <div class="modal-content">
                <span class="close" onclick="cerrarModalJurados()">&times;</span>
                <h3>Invitar Jurados</h3>
                <div class="form-group">
                    <label for="nombres-jurados">Nombres de los Jurados (separados por comas)</label>
                    <input type="text" id="nombres-jurados" placeholder="Jurado 1, Jurado 2, Jurado 3...">
                </div>
                <button onclick="confirmarInvitarJurados()">Invitar Jurados</button>
            </div>
        </div>
        
        <div id="install-banner" class="install-banner" style="display:none;">
            <div>Instala esta aplicación en tu dispositivo para un acceso rápido</div>
            <button onclick="installApp()">Instalar Ahora</button>
        </div>
    </div>
    
    <div id="notification" class="notification"></div>
    
    <script>
        // Contraseña del organizador
        const ORGANIZADOR_PASSWORD = 'tauro360';
        
        // Base de datos local
        let eventos = JSON.parse(localStorage.getItem('eventos')) || [];
        let jurados = JSON.parse(localStorage.getItem('jurados')) || [];
        let puntuaciones = JSON.parse(localStorage.getItem('puntuaciones')) || {};
        let puntuacionesFinal = JSON.parse(localStorage.getItem('puntuacionesFinal')) || {};
        let eventoActual = null;
        let juradoActual = null;
        let deferredPrompt = null;
        
        // Al cargar la página, si hay un evento actual seleccionado, cargarlo
        window.onload = function() {
            const eventoActualId = localStorage.getItem('eventoActualId');
            if (eventoActualId) {
                eventoActual = eventos.find(e => e.id == eventoActualId);
            }
        };
        
        // Registrar Service Worker para PWA
        if ('serviceWorker' in navigator) {
            navigator.serviceWorker.register('data:application/javascript;base64,c2VsZi5hZGRFdmVudExpc3RlbmVyKCdpbnN0YWxsJywgZnVuY3Rpb24oZXZlbnQpIHsKICBzZWxmLnNraXBXYWl0aW5nKCk7Cn0pOwoKc2VsZi5hZGRFdmVudExpc3RlbmVyKCJmZXRjaCIsIGZ1bmN0aW9uKGV2ZW50KSB7CiAgZXZlbnQucmVzcG9uZFdpdGgoCiAgICBjYWNoZXMubWF0Y2goZXZlbnQucmVxdWVzdCkKICAgIC50aGVuKGZ1bmN0aW9uKHJlc3BvbnNlKSB7CiAgICAgIHJldHVybiByZXNwb25zZSB8fCBmZXRjaChldmVudC5yZXF1ZXN0KTsKICAgIH0pCiAgKTsKfSk7');
        }
        
        // Detectar si la app puede instalarse
        window.addEventListener('beforeinstallprompt', (e) => {
            e.preventDefault();
            deferredPrompt = e;
            document.getElementById('install-banner').style.display = 'block';
        });
        
        // Función para instalar la app
        function installApp() {
            if (deferredPrompt) {
                deferredPrompt.prompt();
                deferredPrompt.userChoice.then((choiceResult) => {
                    if (choiceResult.outcome === 'accepted') {
                        showNotification('Aplicación instalada correctamente');
                    }
                    deferredPrompt = null;
                    document.getElementById('install-banner').style.display = 'none';
                });
            }
        }
        
        // Función para mostrar notificaciones
        function showNotification(message, isError = false) {
            const notification = document.getElementById('notification');
            notification.textContent = message;
            notification.className = isError ? 'notification error' : 'notification';
            notification.style.display = 'block';
            
            setTimeout(() => {
                notification.style.display = 'none';
            }, 3000);
        }
        
        // Funciones para mostrar pantallas
        function showScreen(screenId) {
            document.querySelectorAll('.screen').forEach(screen => {
                screen.classList.remove('active');
            });
            document.getElementById(screenId).classList.add('active');
        }
        
        function showAccessScreen() {
            showScreen('access-screen');
        }
        
        function showOrganizadorLogin() {
            showScreen('organizador-login-screen');
        }
        
        function showJuradoAccess() {
            showScreen('jurado-access-screen');
        }
        
        // Función de login del organizador
        function loginOrganizador() {
            const password = document.getElementById('password').value;
            
            if (password === ORGANIZADOR_PASSWORD) {
                showScreen('organizador-screen');
                mostrarEventos();
                actualizarDebugPanel();
                showNotification('Bienvenido Organizador');
            } else {
                showNotification('Contraseña incorrecta', true);
            }
        }
        
        // Función de logout
        function logout() {
            showScreen('access-screen');
            document.getElementById('password').value = '';
            showNotification('Sesión cerrada');
        }
        
        // Función de logout para jurado
        function logoutJurado() {
            showScreen('jurado-access-screen');
            document.getElementById('codigo-acceso').value = '';
            showNotification('Sesión cerrada');
        }
        
        // Función para actualizar el panel de depuración
        function actualizarDebugPanel() {
            document.getElementById('debug-eventos').textContent = eventos.length;
            document.getElementById('debug-jurados').textContent = jurados.length;
            document.getElementById('debug-puntuaciones').textContent = Object.keys(puntuaciones).length;
        }
        
        // Función para limpiar todos los datos
        function limpiarDatos() {
            if (confirm('¿Estás seguro de que quieres eliminar todos los datos? Esta acción no se puede deshacer.')) {
                // Limpiar todas las variables
                eventos = [];
                jurados = [];
                puntuaciones = {};
                puntuacionesFinal = {};
                eventoActual = null;
                juradoActual = null;
                
                // Limpiar localStorage
                localStorage.clear();
                
                // Actualizar la interfaz
                actualizarDebugPanel();
                mostrarEventos();
                showNotification('Todos los datos han sido eliminados');
            }
        }
        
        // Función para mostrar la lista de eventos
        function mostrarEventos() {
            const contenedor = document.getElementById('eventos-lista');
            contenedor.innerHTML = '';
            
            if (eventos.length === 0) {
                contenedor.innerHTML = '<p>No hay eventos creados</p>';
                return;
            }
            
            eventos.forEach(evento => {
                const eventoDiv = document.createElement('div');
                eventoDiv.className = 'evento-card';
                
                const titulo = document.createElement('h4');
                titulo.textContent = evento.nombre;
                
                // Determinar estado del evento
                let estado = '';
                let estadoClass = '';
                if (evento.resultadoFinal && evento.resultadoFinal.length > 0) {
                    estado = 'Completado';
                    estadoClass = 'estado-completado';
                } else if (evento.finalistas && evento.finalistas.length > 0) {
                    estado = 'Final';
                    estadoClass = 'estado-final';
                } else {
                    estado = 'Activo';
                    estadoClass = 'estado-activo';
                }
                
                const estadoSpan = document.createElement('span');
                estadoSpan.className = `evento-estado ${estadoClass}`;
                estadoSpan.textContent = estado;
                titulo.appendChild(estadoSpan);
                
                eventoDiv.appendChild(titulo);
                
                const info = document.createElement('p');
                info.textContent = `Creado el ${new Date(evento.id).toLocaleString()}`;
                eventoDiv.appendChild(info);
                
                const botones = document.createElement('div');
                botones.className = 'evento-actions';
                
                const btnSeleccionar = document.createElement('button');
                btnSeleccionar.textContent = 'Seleccionar';
                btnSeleccionar.className = 'btn-small';
                btnSeleccionar.onclick = () => seleccionarEvento(evento.id);
                botones.appendChild(btnSeleccionar);
                
                const btnEliminar = document.createElement('button');
                btnEliminar.textContent = 'Eliminar';
                btnEliminar.className = 'btn-small btn-secondary';
                // Usamos una función anónima para asegurar que se capture correctamente el ID del evento
                btnEliminar.onclick = (function(id) {
                    return function() {
                        eliminarEvento(id);
                    };
                })(evento.id);
                botones.appendChild(btnEliminar);
                
                eventoDiv.appendChild(botones);
                contenedor.appendChild(eventoDiv);
            });
        }
        
        // Función para mostrar la pantalla de crear evento
        function showCrearEvento() {
            showScreen('crear-evento-screen');
            actualizarParticipantes();
        }
        
        // Función para seleccionar un evento
        function seleccionarEvento(eventoId) {
            eventoActual = eventos.find(e => e.id === eventoId);
            localStorage.setItem('eventoActualId', eventoId);
            
            // Ir a la pantalla de gestión del evento
            showScreen('evento-gestion-screen');
            cargarEventoGestion();
        }
        
        // Función para eliminar un evento - CORREGIDA
        function eliminarEvento(eventoId) {
            console.log('Intentando eliminar evento con ID:', eventoId);
            
            if (!eventoId) {
                console.error('ID de evento no válido');
                showNotification('Error: ID de evento no válido', true);
                return;
            }
            
            if (confirm('¿Estás seguro de que quieres eliminar este evento? Esta acción no se puede deshacer.')) {
                try {
                    console.log('Eliminando evento...');
                    
                    // Eliminar evento
                    eventos = eventos.filter(e => e.id !== eventoId);
                    console.log('Eventos después de eliminar:', eventos);
                    
                    // Eliminar jurados del evento
                    jurados = jurados.filter(j => j.eventoId !== eventoId);
                    console.log('Jurados después de eliminar:', jurados);
                    
                    // Eliminar puntuaciones del evento
                    delete puntuaciones[eventoId];
                    delete puntuacionesFinal[eventoId];
                    console.log('Puntuaciones después de eliminar:', puntuaciones);
                    
                    // Guardar en localStorage
                    localStorage.setItem('eventos', JSON.stringify(eventos));
                    localStorage.setItem('jurados', JSON.stringify(jurados));
                    localStorage.setItem('puntuaciones', JSON.stringify(puntuaciones));
                    localStorage.setItem('puntuacionesFinal', JSON.stringify(puntuacionesFinal));
                    console.log('LocalStorage actualizado');
                    
                    // Si era el evento actual, limpiar
                    if (eventoActual && eventoActual.id === eventoId) {
                        eventoActual = null;
                        localStorage.removeItem('eventoActualId');
                        console.log('Evento actual limpiado');
                    }
                    
                    // Actualizar lista de eventos
                    mostrarEventos();
                    actualizarDebugPanel();
                    showNotification('Evento eliminado correctamente');
                    
                    console.log('Evento eliminado exitosamente');
                } catch (error) {
                    console.error('Error al eliminar evento:', error);
                    showNotification('Error al eliminar el evento: ' + error.message, true);
                }
            } else {
                console.log('Eliminación cancelada por el usuario');
            }
        }
        
        // Función para volver a la lista de eventos
        function volverAEventos() {
            showScreen('organizador-screen');
            mostrarEventos();
        }
        
        // Función para volver a la gestión del evento
        function volverAGestion() {
            showScreen('evento-gestion-screen');
            cargarEventoGestion();
        }
        
        // Función para cargar la gestión del evento
        function cargarEventoGestion() {
            if (!eventoActual) return;
            
            document.getElementById('evento-titulo').textContent = eventoActual.nombre;
            
            // Mostrar detalles del evento
            const detalles = document.getElementById('evento-detalles');
            detalles.innerHTML = `
                <p><strong>Tipo:</strong> ${eventoActual.tipo === 'normal' ? 'Normal (3 toros)' : 'Extra (4 toros)'}</p>
                <p><strong>Participantes:</strong> ${eventoActual.participantes}</p>
                <p><strong>Fecha de creación:</strong> ${new Date(eventoActual.id).toLocaleString()}</p>
            `;
            
            // Mostrar órdenes de toros
            mostrarOrdenesTorosGestion();
            
            // Mostrar jurados
            mostrarJuradosGestion();
            
            // Verificar si se puede generar la final
            verificarSiPuedeGenerarFinal();
            
            // Verificar si hay resultados finales
            if (eventoActual.resultadoFinal && eventoActual.resultadoFinal.length > 0) {
                document.getElementById('ver-resultados-btn').style.display = 'block';
            } else {
                document.getElementById('ver-resultados-btn').style.display = 'none';
            }
        }
        
        // Función para mostrar órdenes de toros en gestión
        function mostrarOrdenesTorosGestion() {
            const contenedor = document.getElementById('ordenes-toros-gestion');
            contenedor.innerHTML = '';
            
            eventoActual.toros.forEach((toro, index) => {
                const toroDiv = document.createElement('div');
                toroDiv.className = 'toro-orden';
                
                const titulo = document.createElement('h4');
                titulo.textContent = `Toro ${index + 1}`;
                toroDiv.appendChild(titulo);
                
                const ordenList = document.createElement('div');
                ordenList.className = 'orden-list';
                
                toro.forEach((participante, pos) => {
                    const item = document.createElement('div');
                    item.className = 'orden-item';
                    item.textContent = `${pos + 1}. ${participante}`;
                    ordenList.appendChild(item);
                });
                
                toroDiv.appendChild(ordenList);
                contenedor.appendChild(toroDiv);
            });
            
            // Mostrar tabla de posiciones por toro
            const posicionesDiv = document.createElement('div');
            posicionesDiv.className = 'posiciones-toros';
            
            const tituloPosiciones = document.createElement('h4');
            tituloPosiciones.textContent = 'Posiciones por Toro';
            posicionesDiv.appendChild(tituloPosiciones);
            
            const tabla = document.createElement('table');
            tabla.className = 'posiciones-toros-table';
            
            // Crear encabezado
            const thead = document.createElement('thead');
            const headerRow = document.createElement('tr');
            
            const thParticipante = document.createElement('th');
            thParticipante.textContent = 'Participante';
            headerRow.appendChild(thParticipante);
            
            eventoActual.toros.forEach((toro, index) => {
                const th = document.createElement('th');
                th.textContent = `Toro ${index + 1}`;
                headerRow.appendChild(th);
            });
            
            thead.appendChild(headerRow);
            tabla.appendChild(thead);
            
            // Crear cuerpo
            const tbody = document.createElement('tbody');
            
            eventoActual.ordenToro1.forEach(participante => {
                const row = document.createElement('tr');
                
                // Nombre del participante
                const tdNombre = document.createElement('td');
                tdNombre.className = 'participante-nombre';
                tdNombre.textContent = participante;
                row.appendChild(tdNombre);
                
                // Posición en cada toro
                eventoActual.toros.forEach((toro, toroIndex) => {
                    const td = document.createElement('td');
                    const posicion = toro.indexOf(participante) + 1;
                    td.textContent = posicion;
                    row.appendChild(td);
                });
                
                tbody.appendChild(row);
            });
            
            tabla.appendChild(tbody);
            posicionesDiv.appendChild(tabla);
            contenedor.appendChild(posicionesDiv);
        }
        
        // Función para mostrar jurados en gestión
        function mostrarJuradosGestion() {
            const contenedor = document.getElementById('jurados-gestion');
            contenedor.innerHTML = '';
            
            if (eventoActual.jurados.length === 0) {
                contenedor.innerHTML = '<p>No hay jurados invitados</p>';
                return;
            }
            
            eventoActual.jurados.forEach(jurado => {
                const juradoCard = document.createElement('div');
                juradoCard.className = 'jurado-card';
                
                const juradoInfo = document.createElement('div');
                juradoInfo.className = 'jurado-name';
                juradoInfo.textContent = jurado.nombre;
                
                const juradoCode = document.createElement('div');
                juradoCode.className = 'jurado-code';
                juradoCode.textContent = jurado.id;
                
                juradoCard.appendChild(juradoInfo);
                juradoCard.appendChild(juradoCode);
                contenedor.appendChild(juradoCard);
            });
        }
        
        // Función para verificar si se puede generar la final
        function verificarSiPuedeGenerarFinal() {
            // Verificar si ya se generó la final
            if (eventoActual.finalistas && eventoActual.finalistas.length > 0) {
                document.getElementById('generar-final-btn').style.display = 'none';
                return;
            }
            
            // Verificar si todos los toros han sido puntuados por todos los jurados
            let todosPuntuaron = true;
            
            eventoActual.toros.forEach((toro, index) => {
                const toroKey = `toro${index + 1}`;
                
                if (!puntuaciones[eventoActual.id] || !puntuaciones[eventoActual.id][toroKey]) {
                    todosPuntuaron = false;
                    return;
                }
                
                // Verificar que cada jurado ha puntuado este toro
                eventoActual.jurados.forEach(jurado => {
                    if (!puntuaciones[eventoActual.id][toroKey][jurado.id]) {
                        todosPuntuaron = false;
                    }
                });
            });
            
            if (todosPuntuaron) {
                document.getElementById('generar-final-btn').style.display = 'block';
            } else {
                document.getElementById('generar-final-btn').style.display = 'none';
            }
        }
        
        // Función para mostrar la pantalla de generar final
        function mostrarGenerarFinal() {
            showScreen('generar-final-screen');
            cargarSeleccionFinalistas();
        }
        
        // Función para cargar la selección de finalistas
        function cargarSeleccionFinalistas() {
            // Calcular clasificación actual
            calcularClasificacion();
            
            const contenedor = document.getElementById('finalistas-seleccion');
            contenedor.innerHTML = '';
            
            // Mostrar los 4 primeros clasificados
            const top4 = eventoActual.clasificacion.slice(0, 4);
            
            top4.forEach((item, index) => {
                const finalistaDiv = document.createElement('div');
                finalistaDiv.className = 'finalista-item';
                
                const position = document.createElement('div');
                position.className = 'finalista-position';
                position.textContent = index + 1;
                
                const name = document.createElement('div');
                name.textContent = item.participante;
                
                finalistaDiv.appendChild(position);
                finalistaDiv.appendChild(name);
                contenedor.appendChild(finalistaDiv);
            });
            
            // Si hay empate en el 4º puesto, mostrar los empatados
            if (eventoActual.clasificacion.length > 4) {
                const cuarto = top4[3];
                const empatados = eventoActual.clasificacion.filter(item => item.puntuacion === cuarto.puntuacion && item.participante !== cuarto.participante);
                
                if (empatados.length > 0) {
                    const empateSelector = document.getElementById('empate-selector');
                    empateSelector.style.display = 'block';
                    
                    const empateOptions = document.getElementById('empate-options');
                    empateOptions.innerHTML = '';
                    
                    // Añadir el 4º actual como opción
                    const actualOption = document.createElement('div');
                    actualOption.className = 'empate-option selected';
                    actualOption.textContent = cuarto.participante;
                    actualOption.dataset.participante = cuarto.participante;
                    actualOption.onclick = () => seleccionarCuartoEmpatado(cuarto.participante);
                    empateOptions.appendChild(actualOption);
                    
                    // Añadir los empatados
                    empatados.forEach(item => {
                        const empateOption = document.createElement('div');
                        empateOption.className = 'empate-option';
                        empateOption.textContent = item.participante;
                        empateOption.dataset.participante = item.participante;
                        empateOption.onclick = () => seleccionarCuartoEmpatado(item.participante);
                        empateOptions.appendChild(empateOption);
                    });
                } else {
                    document.getElementById('empate-selector').style.display = 'none';
                }
            } else {
                document.getElementById('empate-selector').style.display = 'none';
            }
        }
        
        // Función para seleccionar el 4º en caso de empate
        function seleccionarCuartoEmpatado(participante) {
            // Actualizar la selección visual
            document.querySelectorAll('.empate-option').forEach(option => {
                option.classList.remove('selected');
                if (option.dataset.participante === participante) {
                    option.classList.add('selected');
                }
            });
            
            // Reemplazar el 4º clasificado por el seleccionado
            eventoActual.clasificacion[3] = { participante, puntuacion: eventoActual.clasificacion[3].puntuacion };
        }
        
        // Función para confirmar la final
        function confirmarFinal() {
            // Asignar los finalistas
            eventoActual.finalistas = eventoActual.clasificacion.slice(0, 4).map(item => item.participante);
            
            // Guardar el evento
            eventos = eventos.map(e => e.id === eventoActual.id ? eventoActual : e);
            localStorage.setItem('eventos', JSON.stringify(eventos));
            
            // Notificar a los jurados (la próxima vez que entren, verán la final)
            showNotification('Final generada correctamente. Los jurados ya pueden puntuar.');
            
            // Volver a la gestión
            volverAGestion();
        }
        
        // Función para actualizar la lista de participantes según el número seleccionado
        function actualizarParticipantes() {
            const numParticipantes = parseInt(document.getElementById('evento-participantes').value);
            const contenedor = document.getElementById('participantes-lista');
            contenedor.innerHTML = '';
            
            for (let i = 1; i <= numParticipantes; i++) {
                const participanteDiv = document.createElement('div');
                participanteDiv.className = 'participante-item';
                
                const numberDiv = document.createElement('div');
                numberDiv.className = 'participante-number';
                numberDiv.textContent = i;
                
                const nameInput = document.createElement('input');
                nameInput.type = 'text';
                nameInput.id = `participante-${i}`;
                nameInput.placeholder = `Nombre del participante ${i}`;
                nameInput.className = 'participante-name';
                
                participanteDiv.appendChild(numberDiv);
                participanteDiv.appendChild(nameInput);
                contenedor.appendChild(participanteDiv);
            }
        }
        
        // Función para crear un nuevo evento
        function crearEvento() {
            const nombre = document.getElementById('evento-nombre').value;
            const tipo = document.getElementById('evento-tipo').value;
            const participantes = parseInt(document.getElementById('evento-participantes').value);
            
            // Recoger nombres de participantes
            const ordenToro1 = [];
            for (let i = 1; i <= participantes; i++) {
                const nombreParticipante = document.getElementById(`participante-${i}`).value.trim();
                if (!nombreParticipante) {
                    showNotification(`Por favor ingresa el nombre del participante ${i}`, true);
                    return;
                }
                ordenToro1.push(nombreParticipante);
            }
            
            // Generar órdenes para los demás toros según el reglamento
            const toros = generarOrdenes(tipo, participantes, ordenToro1);
            
            // Crear el evento
            const nuevoEvento = {
                id: Date.now(),
                nombre,
                tipo,
                participantes,
                ordenToro1,
                toros,
                jurados: [],
                finalistas: [],
                resultadoFinal: []
            };
            
            eventos.push(nuevoEvento);
            localStorage.setItem('eventos', JSON.stringify(eventos));
            
            // Seleccionar el nuevo evento
            eventoActual = nuevoEvento;
            localStorage.setItem('eventoActualId', nuevoEvento.id);
            
            // Ir a la gestión del evento
            showScreen('evento-gestion-screen');
            cargarEventoGestion();
            
            actualizarDebugPanel();
            showNotification('Evento creado correctamente');
        }
        
        // Función para generar órdenes según el reglamento
        function generarOrdenes(tipo, numParticipantes, ordenToro1) {
            const toros = [ordenToro1];
            
            if (tipo === 'normal') {
                if (numParticipantes === 9) {
                    // 9 participantes - 3 grupos de 3
                    const g1 = ordenToro1.slice(0, 3);
                    const g2 = ordenToro1.slice(3, 6);
                    const g3 = ordenToro1.slice(6, 9);
                    
                    // Toro 2: G3, G1, G2
                    toros.push([...g3, ...g1, ...g2]);
                    
                    // Toro 3: G2, G3, G1
                    toros.push([...g2, ...g3, ...g1]);
                } else if (numParticipantes === 12) {
                    // 12 participantes - 4 grupos de 3
                    const g1 = ordenToro1.slice(0, 3);
                    const g2 = ordenToro1.slice(3, 6);
                    const g3 = ordenToro1.slice(6, 9);
                    const g4 = ordenToro1.slice(9, 12);
                    
                    // Toro 2: G2, G3, G4, G1
                    toros.push([...g2, ...g3, ...g4, ...g1]);
                    
                    // Toro 3: G3, G4, G1, G2
                    toros.push([...g3, ...g4, ...g1, ...g2]);
                }
            } else if (tipo === 'extra') {
                if (numParticipantes === 12) {
                    // 12 participantes - 4 grupos de 3
                    const g1 = ordenToro1.slice(0, 3);
                    const g2 = ordenToro1.slice(3, 6);
                    const g3 = ordenToro1.slice(6, 9);
                    const g4 = ordenToro1.slice(9, 12);
                    
                    // Toro 2: G2, G3, G4, G1
                    toros.push([...g2, ...g3, ...g4, ...g1]);
                    
                    // Toro 3: G3, G4, G1, G2
                    toros.push([...g3, ...g4, ...g1, ...g2]);
                    
                    // Toro 4: G4, G1, G2, G3
                    toros.push([...g4, ...g1, ...g2, ...g3]);
                } else if (numParticipantes === 16) {
                    // 16 participantes - 4 grupos de 4
                    const g1 = ordenToro1.slice(0, 4);
                    const g2 = ordenToro1.slice(4, 8);
                    const g3 = ordenToro1.slice(8, 12);
                    const g4 = ordenToro1.slice(12, 16);
                    
                    // Toro 2: G2, G3, G4, G1
                    toros.push([...g2, ...g3, ...g4, ...g1]);
                    
                    // Toro 3: G3, G4, G1, G2
                    toros.push([...g3, ...g4, ...g1, ...g2]);
                    
                    // Toro 4: G4, G1, G2, G3
                    toros.push([...g4, ...g1, ...g2, ...g3]);
                }
            }
            
            return toros;
        }
        
        // Función para invitar jurados
        function invitarJurados() {
            document.getElementById('juradosModal').style.display = 'block';
            document.getElementById('nombres-jurados').value = '';
        }
        
        // Función para cerrar el modal de jurados
        function cerrarModalJurados() {
            document.getElementById('juradosModal').style.display = 'none';
        }
        
        // Función para confirmar la invitación de jurados
        function confirmarInvitarJurados() {
            const nombres = document.getElementById('nombres-jurados').value.trim();
            
            if (!nombres) {
                showNotification('Por favor ingresa al menos un nombre de jurado', true);
                return;
            }
            
            const listaNombres = nombres.split(',').map(n => n.trim()).filter(n => n);
            
            if (listaNombres.length === 0) {
                showNotification('Por favor ingresa al menos un nombre de jurado', true);
                return;
            }
            
            listaNombres.forEach(nombre => {
                const codigo = Math.random().toString(36).substring(2, 8).toUpperCase();
                
                // Guardar jurado
                const jurado = {
                    id: codigo,
                    nombre,
                    eventoId: eventoActual.id
                };
                
                jurados.push(jurado);
                eventoActual.jurados.push(jurado);
            });
            
            // Guardar en localStorage
            localStorage.setItem('jurados', JSON.stringify(jurados));
            eventos = eventos.map(e => e.id === eventoActual.id ? eventoActual : e);
            localStorage.setItem('eventos', JSON.stringify(eventos));
            
            // Cerrar modal
            cerrarModalJurados();
            
            // Actualizar la vista
            mostrarJuradosGestion();
            actualizarDebugPanel();
            showNotification('Jurados invitados correctamente');
        }
        
        // Función para que un jurado acceda
        function accederJurado() {
            const codigo = document.getElementById('codigo-acceso').value.toUpperCase();
            
            if (!codigo) {
                showNotification('Por favor ingresa tu código de acceso', true);
                return;
            }
            
            // Buscar jurado por código
            juradoActual = jurados.find(j => j.id === codigo);
            
            if (!juradoActual) {
                showNotification('Código de acceso inválido', true);
                return;
            }
            
            // Buscar evento del jurado
            eventoActual = eventos.find(e => e.id === juradoActual.eventoId);
            
            if (!eventoActual) {
                showNotification('Evento no encontrado', true);
                return;
            }
            
            // Verificar si hay final lista para puntuar
            if (eventoActual.finalistas.length > 0) {
                // Verificar si el jurado ya puntuó la final
                let yaPuntuoFinal = false;
                if (puntuacionesFinal[eventoActual.id] && puntuacionesFinal[eventoActual.id][juradoActual.id]) {
                    yaPuntuoFinal = true;
                }
                
                if (!yaPuntuoFinal) {
                    showScreen('jurado-final-screen');
                    cargarFinalJurado();
                    showNotification(`Bienvenido ${juradoActual.nombre}. Puntuación de final disponible.`);
                } else {
                    showScreen('jurado-screen');
                    cargarToro();
                    showNotification(`Bienvenido ${juradoActual.nombre}. Ya has puntuado la final.`);
                }
            } else {
                showScreen('jurado-screen');
                cargarToro();
                showNotification(`Bienvenido ${juradoActual.nombre}`);
            }
        }
        
        // Función para cargar un toro para puntuar
        function cargarToro() {
            // Mostrar información del jurado
            document.getElementById('jurado-nombre').textContent = juradoActual.nombre;
            document.getElementById('jurado-evento').textContent = eventoActual.nombre;
            
            const toroSelect = document.getElementById('toro-select');
            const toroIndex = parseInt(toroSelect.value.replace('toro', '')) - 1;
            
            if (toroIndex >= eventoActual.toros.length) {
                document.getElementById('puntuaciones-form').innerHTML = '';
                return;
            }
            
            const toro = eventoActual.toros[toroIndex];
            const contenedor = document.getElementById('puntuaciones-form');
            contenedor.innerHTML = '';
            
            // Crear tabla de puntuaciones
            const table = document.createElement('table');
            table.className = 'puntuacion-table';
            
            // Encabezado
            const thead = document.createElement('thead');
            const headerRow = document.createElement('tr');
            
            const thOrden = document.createElement('th');
            thOrden.textContent = 'Orden';
            headerRow.appendChild(thOrden);
            
            const thNombre = document.createElement('th');
            thNombre.textContent = 'Recortador';
            headerRow.appendChild(thNombre);
            
            const thPuntuacion = document.createElement('th');
            thPuntuacion.textContent = 'Puntuación';
            headerRow.appendChild(thPuntuacion);
            
            thead.appendChild(headerRow);
            table.appendChild(thead);
            
            // Cuerpo
            const tbody = document.createElement('tbody');
            
            toro.forEach((participante, index) => {
                const row = document.createElement('tr');
                
                const tdOrden = document.createElement('td');
                tdOrden.textContent = index + 1;
                row.appendChild(tdOrden);
                
                const tdNombre = document.createElement('td');
                tdNombre.textContent = participante;
                row.appendChild(tdNombre);
                
                const tdPuntuacion = document.createElement('td');
                const input = document.createElement('input');
                input.type = 'number';
                input.min = '0';
                input.max = '10';
                input.step = '0.1';
                input.placeholder = '0.0';
                input.id = `puntuacion-${participante}`;
                
                // Si ya hay puntuaciones guardadas, cargarlas
                if (puntuaciones[eventoActual.id] && 
                    puntuaciones[eventoActual.id][toroSelect.value] && 
                    puntuaciones[eventoActual.id][toroSelect.value][juradoActual.id] &&
                    puntuaciones[eventoActual.id][toroSelect.value][juradoActual.id][participante]) {
                    input.value = puntuaciones[eventoActual.id][toroSelect.value][juradoActual.id][participante];
                }
                
                tdPuntuacion.appendChild(input);
                row.appendChild(tdPuntuacion);
                
                tbody.appendChild(row);
            });
            
            table.appendChild(tbody);
            contenedor.appendChild(table);
        }
        
        // Función para guardar puntuaciones de un toro
        function guardarPuntuaciones() {
            const toroSelect = document.getElementById('toro-select');
            const toro = toroSelect.value;
            const toroIndex = parseInt(toro.replace('toro', '')) - 1;
            
            if (toroIndex >= eventoActual.toros.length) {
                showNotification('Toro no válido', true);
                return;
            }
            
            const participantes = eventoActual.toros[toroIndex];
            const puntuacionesToro = {};
            
            let allValid = true;
            
            participantes.forEach(participante => {
                const input = document.getElementById(`puntuacion-${participante}`);
                const puntuacion = parseFloat(input.value);
                
                if (isNaN(puntuacion) || puntuacion < 0 || puntuacion > 10) {
                    allValid = false;
                    return;
                }
                
                puntuacionesToro[participante] = puntuacion;
            });
            
            if (!allValid) {
                showNotification('Por favor ingresa puntuaciones válidas (0-10)', true);
                return;
            }
            
            // Guardar puntuaciones
            if (!puntuaciones[eventoActual.id]) {
                puntuaciones[eventoActual.id] = {};
            }
            
            if (!puntuaciones[eventoActual.id][toro]) {
                puntuaciones[eventoActual.id][toro] = {};
            }
            
            puntuaciones[eventoActual.id][toro][juradoActual.id] = puntuacionesToro;
            localStorage.setItem('puntuaciones', JSON.stringify(puntuaciones));
            
            actualizarDebugPanel();
            showNotification('Puntuaciones guardadas correctamente');
            
            // Pasar al siguiente toro si existe
            const nextToroIndex = toroIndex + 1;
            if (nextToroIndex < eventoActual.toros.length) {
                toroSelect.value = `toro${nextToroIndex + 1}`;
                cargarToro();
            }
            
            // Verificar si todos los jurados han puntuado todos los toros
            verificarTodosPuntuaron();
        }
        
        // Función para verificar si todos los jurados han puntuado todos los toros
        function verificarTodosPuntuaron() {
            let todosPuntuaron = true;
            
            eventoActual.toros.forEach((toro, index) => {
                const toroKey = `toro${index + 1}`;
                
                if (!puntuaciones[eventoActual.id] || !puntuaciones[eventoActual.id][toroKey]) {
                    todosPuntuaron = false;
                    return;
                }
                
                // Verificar que cada jurado ha puntuado este toro
                eventoActual.jurados.forEach(jurado => {
                    if (!puntuaciones[eventoActual.id][toroKey][jurado.id]) {
                        todosPuntuaron = false;
                    }
                });
            });
            
            // Si todos puntuaron, generar automáticamente la clasificación
            if (todosPuntuaron && eventoActual.jurados.length > 0) {
                calcularClasificacion();
                showNotification('Todos los jurados han puntuado. Clasificación generada automáticamente.');
            }
        }
        
        // Función para cargar la final para el jurado
        function cargarFinalJurado() {
            // Mostrar información del jurado
            document.getElementById('jurado-nombre-final').textContent = juradoActual.nombre;
            document.getElementById('jurado-evento-final').textContent = eventoActual.nombre;
            
            const tbody = document.getElementById('final-puntuaciones-tbody');
            tbody.innerHTML = '';
            
            eventoActual.finalistas.forEach((finalista, index) => {
                const row = document.createElement('tr');
                
                // Posición
                const tdPosicion = document.createElement('td');
                tdPosicion.textContent = index + 1;
                row.appendChild(tdPosicion);
                
                // Nombre del finalista
                const tdNombre = document.createElement('td');
                tdNombre.textContent = finalista;
                row.appendChild(tdNombre);
                
                // Rondas de puntuación
                for (let ronda = 1; ronda <= 7; ronda++) {
                    const td = document.createElement('td');
                    const input = document.createElement('input');
                    input.type = 'number';
                    input.min = '0';
                    input.max = '10';
                    input.step = '0.1';
                    input.placeholder = '0.0';
                    input.id = `final-${finalista}-ronda${ronda}`;
                    
                    // Si ya hay puntuaciones guardadas, cargarlas
                    if (puntuacionesFinal[eventoActual.id] && 
                        puntuacionesFinal[eventoActual.id][juradoActual.id] &&
                        puntuacionesFinal[eventoActual.id][juradoActual.id][finalista] &&
                        puntuacionesFinal[eventoActual.id][juradoActual.id][finalista][ronda - 1]) {
                        input.value = puntuacionesFinal[eventoActual.id][juradoActual.id][finalista][ronda - 1];
                    }
                    
                    td.appendChild(input);
                    row.appendChild(td);
                }
                
                tbody.appendChild(row);
            });
        }
        
        // Función para guardar puntuaciones de la final (nuevo método)
        function guardarPuntuacionesFinalJurado() {
            const puntuacionesFinales = {};
            
            eventoActual.finalistas.forEach(finalista => {
                puntuacionesFinales[finalista] = [];
                
                for (let ronda = 1; ronda <= 7; ronda++) {
                    const input = document.getElementById(`final-${finalista}-ronda${ronda}`);
                    if (input && input.value !== '') {
                        const puntuacion = parseFloat(input.value);
                        if (!isNaN(puntuacion) && puntuacion >= 0 && puntuacion <= 10) {
                            puntuacionesFinales[finalista].push(puntuacion);
                        }
                    }
                }
                
                // Calcular promedio
                if (puntuacionesFinales[finalista].length > 0) {
                    const sum = puntuacionesFinales[finalista].reduce((a, b) => a + b, 0);
                    puntuacionesFinales[finalista] = sum / puntuacionesFinales[finalista].length;
                } else {
                    puntuacionesFinales[finalista] = 0;
                }
            });
            
            // Guardar puntuaciones finales
            if (!puntuacionesFinal[eventoActual.id]) {
                puntuacionesFinal[eventoActual.id] = {};
            }
            
            puntuacionesFinal[eventoActual.id][juradoActual.id] = puntuacionesFinales;
            localStorage.setItem('puntuacionesFinal', JSON.stringify(puntuacionesFinal));
            
            // Verificar si todos los jurados ya puntuaron la final
            verificarTodosJuradosFinal();
            
            actualizarDebugPanel();
            showNotification('Puntuaciones de la final guardadas correctamente');
        }
        
        // Función para verificar si todos los jurados puntuaron la final
        function verificarTodosJuradosFinal() {
            if (!eventoActual.finalistas || eventoActual.finalistas.length === 0) {
                return;
            }
            
            let todosPuntuaron = true;
            
            // Verificar si cada jurado ha puntuado la final
            eventoActual.jurados.forEach(jurado => {
                if (!puntuacionesFinal[eventoActual.id] || !puntuacionesFinal[eventoActual.id][jurado.id]) {
                    todosPuntuaron = false;
                }
            });
            
            // Si todos puntuaron, actualizar el evento
            if (todosPuntuaron) {
                eventos = eventos.map(e => e.id === eventoActual.id ? eventoActual : e);
                localStorage.setItem('eventos', JSON.stringify(eventos));
                
                // Calcular y mostrar resultados finales
                calcularResultadosFinales();
                
                // Mostrar notificación al organizador
                showNotification('Todos los jurados han puntuado la final. Resultados disponibles.');
            }
        }
        
        // Función para ver la clasificación (organizador)
        function verClasificacion() {
            // Calcular clasificación automáticamente
            calcularClasificacion();
            
            // Mostrar pantalla de clasificación
            showScreen('clasificacion-screen');
        }
        
        // Función para calcular la clasificación
        function calcularClasificacion() {
            const puntuacionesAcumuladas = {};
            
            // Inicializar puntuaciones con todos los participantes del evento
            eventoActual.ordenToro1.forEach(participante => {
                puntuacionesAcumuladas[participante] = 0;
            });
            
            // Sumar puntuaciones de cada toro
            eventoActual.toros.forEach((toro, index) => {
                const toroKey = `toro${index + 1}`;
                
                if (puntuaciones[eventoActual.id] && puntuaciones[eventoActual.id][toroKey]) {
                    toro.forEach(participante => {
                        let sumaPuntuaciones = 0;
                        let countJurados = 0;
                        
                        // Sumar puntuaciones de todos los jurados para este participante en este toro
                        Object.values(puntuaciones[eventoActual.id][toroKey]).forEach(puntuacionesJurado => {
                            if (puntuacionesJurado[participante]) {
                                sumaPuntuaciones += puntuacionesJurado[participante];
                                countJurados++;
                            }
                        });
                        
                        // Calcular promedio y sumar a la acumulada
                        if (countJurados > 0) {
                            const promedio = sumaPuntuaciones / countJurados;
                            puntuacionesAcumuladas[participante] += promedio;
                        }
                    });
                }
            });
            
            // Ordenar participantes por puntuación
            eventoActual.clasificacion = Object.entries(puntuacionesAcumuladas)
                .map(([participante, puntuacion]) => ({ participante, puntuacion }))
                .sort((a, b) => b.puntuacion - a.puntuacion);
            
            // Mostrar tabla de clasificación
            const contenedor = document.getElementById('tabla-clasificacion');
            contenedor.innerHTML = '';
            
            const table = document.createElement('table');
            table.className = 'clasificacion-table';
            
            // Encabezado
            const thead = document.createElement('thead');
            const headerRow = document.createElement('tr');
            
            const thPosicion = document.createElement('th');
            thPosicion.textContent = 'Pos';
            headerRow.appendChild(thPosicion);
            
            const thParticipante = document.createElement('th');
            thParticipante.textContent = 'Participante';
            headerRow.appendChild(thParticipante);
            
            const thPuntuacion = document.createElement('th');
            thPuntuacion.textContent = 'Puntos';
            headerRow.appendChild(thPuntuacion);
            
            thead.appendChild(headerRow);
            table.appendChild(thead);
            
            // Cuerpo
            const tbody = document.createElement('tbody');
            
            eventoActual.clasificacion.forEach((item, index) => {
                const row = document.createElement('tr');
                
                if (index < 4) {
                    row.classList.add('finalista');
                }
                
                const tdPosicion = document.createElement('td');
                tdPosicion.textContent = index + 1;
                row.appendChild(tdPosicion);
                
                const tdParticipante = document.createElement('td');
                tdParticipante.textContent = item.participante;
                row.appendChild(tdParticipante);
                
                const tdPuntuacion = document.createElement('td');
                tdPuntuacion.textContent = item.puntuacion.toFixed(2);
                row.appendChild(tdPuntuacion);
                
                tbody.appendChild(row);
            });
            
            table.appendChild(tbody);
            contenedor.appendChild(table);
        }
        
        // Función para ver resultados finales
        function verResultadosFinales() {
            calcularResultadosFinales();
            showScreen('resultados-screen');
        }
        
        // Función para calcular resultados finales
        function calcularResultadosFinales() {
            // Calcular puntuaciones finales de cada jurado
            const puntuacionesFinalesAcumuladas = {};
            
            // Inicializar puntuaciones finales
            eventoActual.finalistas.forEach(finalista => {
                puntuacionesFinalesAcumuladas[finalista] = 0;
            });
            
            // Sumar puntuaciones de la final de todos los jurados
            if (puntuacionesFinal[eventoActual.id]) {
                Object.values(puntuacionesFinal[eventoActual.id]).forEach(puntuacionesJurado => {
                    Object.entries(puntuacionesJurado).forEach(([finalista, puntuacion]) => {
                        puntuacionesFinalesAcumuladas[finalista] += puntuacion;
                    });
                });
                
                // Calcular promedio para cada finalista
                eventoActual.finalistas.forEach(finalista => {
                    puntuacionesFinalesAcumuladas[finalista] /= eventoActual.jurados.length;
                });
            }
            
            // Ordenar finalistas por puntuación final
            eventoActual.resultadoFinal = Object.entries(puntuacionesFinalesAcumuladas)
                .map(([participante, puntuacion]) => ({ participante, puntuacion }))
                .sort((a, b) => b.puntuacion - a.puntuacion);
            
            // Guardar resultado
            eventos = eventos.map(e => e.id === eventoActual.id ? eventoActual : e);
            localStorage.setItem('eventos', JSON.stringify(eventos));
            
            // Mostrar tabla de resultados finales
            const contenedor = document.getElementById('tabla-resultados-finales');
            contenedor.innerHTML = '';
            
            const table = document.createElement('table');
            table.className = 'final-results-table';
            
            // Encabezado
            const thead = document.createElement('thead');
            const headerRow = document.createElement('tr');
            
            const thPosicion = document.createElement('th');
            thPosicion.textContent = 'Posición Final';
            headerRow.appendChild(thPosicion);
            
            const thParticipante = document.createElement('th');
            thParticipante.textContent = 'Participante';
            headerRow.appendChild(thParticipante);
            
            const thPuntuacionClasificacion = document.createElement('th');
            thPuntuacionClasificacion.textContent = 'Puntos Clasificación';
            headerRow.appendChild(thPuntuacionClasificacion);
            
            const thPuntuacionFinal = document.createElement('th');
            thPuntuacionFinal.textContent = 'Puntos Final';
            headerRow.appendChild(thPuntuacionFinal);
            
            thead.appendChild(headerRow);
            table.appendChild(thead);
            
            // Cuerpo
            const tbody = document.createElement('tbody');
            
            eventoActual.resultadoFinal.forEach((item, index) => {
                const row = document.createElement('tr');
                
                if (index === 0) {
                    row.classList.add('ganador-final');
                }
                
                const tdPosicion = document.createElement('td');
                tdPosicion.className = 'posicion-final';
                tdPosicion.textContent = index + 1;
                row.appendChild(tdPosicion);
                
                const tdParticipante = document.createElement('td');
                tdParticipante.textContent = item.participante;
                row.appendChild(tdParticipante);
                
                // Buscar puntuación de clasificación
                const puntuacionClasificacion = eventoActual.clasificacion.find(c => c.participante === item.participante)?.puntuacion || 0;
                
                const tdPuntuacionClasificacion = document.createElement('td');
                tdPuntuacionClasificacion.textContent = puntuacionClasificacion.toFixed(2);
                row.appendChild(tdPuntuacionClasificacion);
                
                const tdPuntuacionFinal = document.createElement('td');
                tdPuntuacionFinal.textContent = item.puntuacion.toFixed(2);
                row.appendChild(tdPuntuacionFinal);
                
                tbody.appendChild(row);
            });
            
            table.appendChild(tbody);
            contenedor.appendChild(table);
        }
        
        // Funciones de exportar e importar eventos
        function exportarEventos() {
            const data = {
                eventos,
                jurados,
                puntuaciones,
                puntuacionesFinal
            };
            
            const blob = new Blob([JSON.stringify(data)], { type: 'application/json' });
            const url = URL.createObjectURL(blob);
            const a = document.createElement('a');
            a.href = url;
            a.download = 'eventos_tauro_esencia.json';
            a.click();
            URL.revokeObjectURL(url);
            
            showNotification('Eventos exportados correctamente');
        }
        
        function importarEventos() {
            document.getElementById('import-file').click();
        }
        
        function handleImport(event) {
            const file = event.target.files[0];
            if (!file) return;
            
            const reader = new FileReader();
            reader.onload = function(e) {
                try {
                    const data = JSON.parse(e.target.result);
                    
                    // Validar que tenga las propiedades necesarias
                    if (data.eventos && data.jurados && data.puntuaciones && data.puntuacionesFinal) {
                        eventos = data.eventos;
                        jurados = data.jurados;
                        puntuaciones = data.puntuaciones;
                        puntuacionesFinal = data.puntuacionesFinal;
                        
                        localStorage.setItem('eventos', JSON.stringify(eventos));
                        localStorage.setItem('jurados', JSON.stringify(jurados));
                        localStorage.setItem('puntuaciones', JSON.stringify(puntuaciones));
                        localStorage.setItem('puntuacionesFinal', JSON.stringify(puntuacionesFinal));
                        
                        actualizarDebugPanel();
                        mostrarEventos();
                        showNotification('Eventos importados correctamente');
                    } else {
                        showNotification('El archivo no tiene el formato correcto', true);
                    }
                } catch (error) {
                    showNotification('Error al importar los eventos', true);
                }
            };
            reader.readAsText(file);
        }
    </script>
</body>
</html>
