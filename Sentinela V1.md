# Sentinel V1 🛡️

> Monitoramento inteligente e autônomo para ambientes críticos, desenvolvido para enfrentar os desafios climáticos do coração do agronegócio brasileiro.

![Status](https://img.shields.io/badge/status-em%20desenvolvimento-yellow) ![Licença](https://img.shields.io/badge/licença-MIT-blue) ![Tecnologia](https://img.shields.io/badge/stack-ESP32%20%7C%20Node.js%20%7C%20React-green)

---

## 📍 Contexto Regional
O **Sentinel V1** nasceu em **Sorriso-MT**, a Capital Nacional do Agronegócio. Devido à intensa atividade agrícola e ao clima característico da região — marcado por períodos de seca extrema e alta concentração de partículas em suspensão (poeira) — identificamos a necessidade de uma solução robusta para monitorar a qualidade do ar e as condições ambientais em tempo real, garantindo a integridade de equipamentos e o bem-estar humano.

## 🚀 Funcionalidades Principais
- **Monitoramento Ambiental:** Sensores de partículas (poeira), umidade, temperatura, ruído e luminosidade.
- **Atuação Automática:** Acionamento inteligente de *coolers* para ventilação e *buzzers* para alertas de segurança.
- **Dashboard em Tempo Real:** Visualização intuitiva dos dados coletados.
- **Alertas Proativos:** Notificações baseadas em limites críticos configuráveis.

## 🛠️ Stack Tecnológica
- **Hardware:** ESP32 (Microcontrolador).
- **Backend:** Node.js com comunicação via MQTT e WebSockets.
- **Frontend:** React (Dashboard interativo).
- **Banco de Dados:** PostgreSQL (Armazenamento de séries temporais).
- **Protocolos:** MQTT para comunicação leve entre dispositivos e servidor.

## 🏗️ Arquitetura
O fluxo de dados segue uma arquitetura orientada a eventos:
1. **Edge:** O ESP32 coleta dados e publica via **MQTT**.
2. **Broker:** O broker gerencia as mensagens em tempo real.
3. **Backend:** O servidor Node.js processa os dados e persiste no **PostgreSQL**.
4. **Dashboard:** O React consome os dados via **WebSockets** para exibição instantânea.

## ⚙️ Como Executar
1. **Clone o repositório:** `git clone https://github.com/seu-usuario/sentinel-v1.git`
2. **Backend:** Navegue até a pasta `/server`, instale as dependências (`npm install`) e execute `npm start`.
3. **Frontend:** Navegue até a pasta `/client`, instale as dependências (`npm install`) e execute `npm run dev`.
4. **Hardware:** Configure o firmware do ESP32 com as credenciais do seu broker MQTT.

## 👤 Autor
**Jonas Gabriel**  
Estudante de Análise e Desenvolvimento de Sistemas (ADS).

## 📝 Licença
Este projeto está sob a licença **MIT**. Consulte o arquivo `LICENSE` para mais detalhes.