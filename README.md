# 🌐 ActiDesk

**🖋️ Autor:** Jean Pierre Andrade Feltran — RM 566534

## 📝 Descrição
ActiDesk é uma pulseira inteligente projetada para reduzir o sedentarismo. O dispositivo monitora movimentos com um acelerômetro e registra temperatura corporal; quando detecta períodos prolongados de inatividade, emite alertas e gera gráficos que ajudam o usuário a entender sua rotina e tomar pequenas ações para melhorar a saúde física e mental.

## 🎥 Demonstração
- Wokwi: https://wokwi.com/projects/447647819843561473  
- Vídeo explicativo: https://youtu.be/fofatwvbKXk

## 🏗️ Arquitetura resumida
- **ESP32** — lê acelerômetro e temperatura e publica dados via **MQTT** no tópico `DinoDadosTech`.
- **Broker MQTT** — `44.223.43.74:1883` (informação fornecida).  
- **Node-RED** — no servidor expõe endpoint HTTP: `http://44.223.43.74:1880/DinoDadosTech` que retorna o último payload recebido.
- **Dashboard (HTML)** — consome o endpoint HTTP e desenha gráficos com HTML e CSS dentro do HTML

- ## 🚀 Imagem do projeto final 
- <img width="1024" height="1536" alt="ChatGPT Image 20 de nov  de 2025, 22_36_07" src="https://github.com/user-attachments/assets/16269c72-1356-4398-b0b6-3595aee66c1a" />
