# TP_EDI_2024
Creamos repositorio para la materia Edi 2024


function colorGenerateRGB() {
    let colors = [];
    for (let i2 = 0; i2 < 3; i2++) {
        colors[i2] = Math.floor((Math.random() * 256));
        // colors.push(Math.floor((Math.random() * 256)));
    }

    return 'rgb(' + colors[0] + ',' + colors[1] + ',' + colors[2] + ')';
    return `rgb(${colors[0]},${colors[1]},${colors[2]})`;
}

function generatePallet(count) {
    let paleta = [];
    for (let i1 = 0; i1 < count; i1++) {
        paleta[i1] = colorGenerateRGB();
    }

    return paleta;
}
//Imprimo paleta

console.log(generatePallet(13));
