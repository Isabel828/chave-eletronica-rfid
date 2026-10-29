# Chave eletrônica com RFID — EmbarcaTech

Projeto acadêmico em C para Raspberry Pi Pico, com leitura de cartões RFID MFRC522, display OLED SSD1306, LEDs de status, buzzers e servo motor para simulação de controle de acesso.

## Funcionalidades
- Leitura do UID de cartões RFID e comparação com usuários cadastrados.
- Feedback de acesso autorizado ou negado via OLED, LEDs e sinal sonoro.
- Acionamento de servo para simular abertura da trava.
- Cadastro de até dez usuários via botão físico (armazenamento em memória, sem persistência).

## Tecnologias
C, Raspberry Pi Pico SDK, CMake, SPI, I2C, PWM, MFRC522 e SSD1306.

## Organização
- `src/main/`: lógica da aplicação.
- `src/rfid/`: leitura RFID.
- `src/display/`: mensagens no OLED.
- `src/lib/`: driver MFRC522.
- `inc/`: suporte ao SSD1306.
- `CMakeLists.txt`: configuração de compilação.

## Compilação
Requer Pico SDK, compilador ARM e CMake configurados. A compilação e o funcionamento no hardware não foram verificados nesta revisão.

## Observações de segurança
Os UIDs de cartões não são autenticação forte, pois podem ser clonados. O projeto é educacional e não deve ser usado como fechadura de segurança real sem medidas adicionais. O UID previamente definido no código foi substituído por um valor ilustrativo para evitar divulgar identificadores de acesso.

## Créditos
Projeto acadêmico de sistemas embarcados. Preserve os créditos dos colaboradores e das bibliotecas utilizadas.
