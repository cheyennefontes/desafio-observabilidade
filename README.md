# Desafio de Observabilidade 

Solução para o Desafio de Observabilidade da O2B Academy. Neste repositório, você encontrará minha implementação prática para configurar um ambiente de observabilidade usando Prometheus e Grafana para monitorar uma aplicação de exemplo em Python.

## Objetivo

O objetivo deste desafio era proporcionar uma experiência prática na configuração de ferramentas populares de observabilidade e entender como monitorar métricas de uma aplicação simples.

## Minha Solução

### Passos Realizados

1. **Instalação do Prometheus, Grafana e Alertmanager:**
   - Clonei o repositório e acessei o diretório do laboratório.
   - Criei um arquivo `docker-compose.yml` para definir os serviços Prometheus, Grafana e Alertmanager.

2. **Configuração da Aplicação de Exemplo:**
   - Certifiquei-me de ter Flask e Prometheus Client Python instalados.
   - Acessei o diretório da aplicação e iniciei a aplicação em Python.

3. **Gerando Métricas na Aplicação:**
   - Acessei a aplicação em http://localhost:3001 e cliquei em "Gerar Erro" e "Calcular Duração".

4. **Configuração do Prometheus:**
   - No arquivo `prometheus.yml` no diretório `prometheus`, adicionei uma seção para coletar métricas da minha aplicação Python.

5. **Integração com o Discord:**
   - No arquivo `alertmanager.yml` no diretório `prometheus`, configurei o Alertmanager para enviar alertas para o Discord.
   - Adicionei um receiver para o Discord com o webhook URL correspondente.

6. **Iniciando o Ambiente de Observabilidade:**
   - Voltei para o diretório raiz do projeto e executei o comando para iniciar os serviços Prometheus e Grafana.

7. **Acessando o Prometheus e Grafana:**
   - Acessei o painel do Prometheus em http://localhost:9090 e verifiquei se estava acessando os dados da minha aplicação.
   - Acessei o painel do Grafana em http://localhost:3000 e fiz login com as credenciais padrão (admin/admin)

