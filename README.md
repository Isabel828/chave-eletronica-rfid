# Chave Eletrônica RFID

Projeto de sistemas embarcados em C para controle de acesso por RFID, utilizando Raspberry Pi Pico, leitor MFRC522 e display OLED SSD1306.

## Tecnologias

- C e Raspberry Pi Pico SDK
- Leitor RFID MFRC522
- Display OLED SSD1306
- CMake

## Estrutura do código-fonte

- `src/main/` — lógica principal da chave eletrônica
- `src/rfid/` — integração com o leitor RFID
- `src/display/` — apresentação no OLED
- `src/lib/` — biblioteca do MFRC522
- `inc/` — drivers e cabeçalhos OLED
- `CMakeLists.txt` — configuração de compilação

## Execução

É necessário configurar o Raspberry Pi Pico SDK e as ferramentas de compilação para a placa. O projeto depende do hardware conectado e não foi validado fisicamente nesta revisão.

## Publicação

**A documentação foi publicada, mas os arquivos de código-fonte ainda estão sendo adicionados ao repositório.** A pasta `build/` e os arquivos temporários não devem ser versionados.

## Segurança

Use apenas cartões de teste autorizados e não publique identificadores reais de credenciais de acesso. A solução é um protótipo acadêmico, não um sistema de segurança certificado.
