const int tempo_atraso = 30; // Tempo de atraso em milissegundos
const int pinStart = 2; // Pino inicial
const int pinEnd = 7;   // Pino final

void setup() {
    // Configura todos os pinos como saída
    for (int i = pinStart; i <= pinEnd; i++) {
        pinMode(i, OUTPUT);
    }
}

void loop() {
    // Pisca os LEDs de cima para baixo
    piscaLEDs(pinEnd, pinStart);
    delay(500); // Espera meio segundo antes de inverter
    // Pisca os LEDs de baixo para cima
    piscaLEDs(pinStart, pinEnd);
    delay(500); // Espera meio segundo antes de reiniciar
}

// Função para piscar os LEDs em uma determinada ordem
void piscaLEDs(int start, int end) {
    for (int i = start; i >= end; i--) {
        digitalWrite(i, HIGH); // Liga o LED
        delay(tempo_atraso);
        digitalWrite(i, LOW);  // Desliga o LED
        delay(tempo_atraso);
    }
}
