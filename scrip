function exportarConfig() {
    const s = JSON.parse(localStorage.getItem('ui_prefs')) || {};
    const contenido = `Configuración de Interfaz:
    --------------------------
    Idioma: ${s.lang || 'es'}
    Fondo Hex: ${s.bg || '#121212'}
    Texto Hex: ${s.text || '#ffffff'}
    Opacidad: ${s.alpha || '0.95'}`;

    const blob = new Blob([contenido], { type: 'text/plain' });
    const url = URL.createObjectURL(blob);
    const a = document.createElement('a');
    a.href = url;
    a.download = 'mi_paleta_colores.txt';
    a.click();
    URL.revokeObjectURL(url);
}
