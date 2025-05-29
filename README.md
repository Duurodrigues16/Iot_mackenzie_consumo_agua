💧 Sistema de Monitoramento Inteligente do Consumo de Água em Hospitais
Este projeto simula um sistema inteligente de monitoramento e controle do uso de água em hospitais, com base na recomendação da ONU de 110L por pessoa/dia. Desenvolvido com ESP32, LCD I2C e comunicação via MQTT, o sistema integra-se à plataforma ThingsBoard Cloud para visualização remota dos dados em tempo real.

🚑 Aplicações no Ambiente Hospitalar
✅ Monitoramento contínuo do consumo de água por setor ou ala hospitalar
🚫 Sistema de bloqueio (válvula simulada) ao atingir o limite diário de uso
🔘 Botão de emergência permite liberações extras de 20L por vez
📟 Display LCD exibe o consumo e status em tempo real
📤 Envio de dados via MQTT para o painel de controle na nuvem
💡 LED sinaliza bloqueio do fluxo por excesso de consumo
📊 Painel de visualização remota com gráficos e alertas para a equipe técnica

🔧 Componentes Utilizados (Simulados)

ESP32 DevKit V1

LCD 16x2 com interface I2C

Módulo Relé (simula controle da válvula de água)

LED Vermelho (indica interrupção do fornecimento)

Botão de liberação de bônus emergencial

Broker MQTT (ThingsBoard Cloud)

🌐 Comunicação MQTT

Broker: mqtt.thingsboard.cloud

Porta: 1883

Tópico: v1/devices/me/telemetry

Usuário (Token do dispositivo): JUAcqz8Sp52UcNl7FlGA

Senha: (deixe em branco)


🖥 Informações no Display LCD

Linha 1: Consumo: XX.XXL

Linha 2: Fluxo: 10.0L/s (simulado)

Ao atingir o limite diário:

Linha 1: Limite atingido

Linha 2: Liberações: N (número de bônus usados)

Ao usar o botão de liberação:

Linha 1: Uso liberado

Linha 2: Bônus #N

🛠 Como Executar no Wokwi

Acesse o simulador Wokwi

Importe os arquivos diagram.json e sketch.ino

Conecte o LCD ao VIN, GND, D21 (SDA) e D22 (SCL)

Inicie a simulação

O sistema irá simular o uso contínuo de água em tempo real

Os dados são enviados automaticamente para o ThingsBoard Cloud

📊 Painel no ThingsBoard Cloud

Crie um dispositivo no ThingsBoard

Copie o token e insira na variável mqtt_username no código

Acompanhe os dados na aba Latest Telemetry

Vídeo: https://youtu.be/R3EnURlIW44

🧠 Finalidade e Contribuições
Este projeto foi desenvolvido com foco educacional e demonstrativo, apresentando conceitos de Internet das Coisas (IoT) aplicados à gestão hídrica hospitalar. A proposta visa promover o uso consciente da água, automação e alertas para evitar desperdícios em ambientes críticos como hospitais. Sugestões e melhorias são muito bem-vindas!

---
