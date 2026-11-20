# FreeLLMAPI - Ambiente de Deploy e Orquestração Docker

## 1. Objetivo e Finalidade
Ambiente de execução containerizado para disponibilização da API FreeLLMAPI, fornecendo inferência e abstração de modelos de linguagem.

## 2. Tecnologias Utilizadas
- Docker, Docker Compose, Bash, YAML

## 3. Arquitetura e Estrutura de Diretórios
Ambiente de implantação baseado em container Docker oficial (`ghcr.io/tashfeenahmed/freellmapi:latest`) com injeção de parâmetros via arquivo `.env`.

## 4. Principais Arquivos e Responsabilidades
- `docker-compose.yml`: Definição de serviços, portas expostas e volumes.
- `.env`: Configuração das chaves de provedores e portas de rede.

## 5. Funcionalidades Identificadas
- Execução em container isolado e escalável
- Roteamento transparente de requisições de LLM
- Fácil inicialização com apenas um comando

## 6. Como Compilar ou Executar
```bash
docker-compose up -d
# Verificar logs: docker-compose logs -f
```

## 7. Estado Atual do Projeto
**Completo**

## 8. Pendências e Limitações Identificadas
Configuração dos tokens dos modelos desejados no arquivo `.env`.
