# Nerdlandia – Infraestrutura Self-Hosted

Projeto acadêmico de infraestrutura web utilizando Docker e SWAG (Nginx), com serviços self-hosted acessíveis via HTTPS.

---

## Tecnologias Utilizadas

<p align="left">
  <img src="https://img.shields.io/badge/Linux-Ubuntu-E95420?logo=ubuntu&logoColor=white" />
  <img src="https://img.shields.io/badge/Docker-Container-2496ED?logo=docker&logoColor=white" />
  <img src="https://img.shields.io/badge/Docker%20Compose-Orquestração-384D54?logo=docker&logoColor=white" />
  <img src="https://img.shields.io/badge/Nginx-Proxy%20Reverso-009639?logo=nginx&logoColor=white" />
  <img src="https://img.shields.io/badge/SWAG-LinuxServer.io-0A0A0A?logo=linux&logoColor=white" />
  <img src="https://img.shields.io/badge/Azure-Virtual%20Machine-0078D4?logo=microsoftazure&logoColor=white" />
</p>

---

## Objetivo
Implantar serviços web em um servidor Linux utilizando Docker, proxy reverso com Nginx (SWAG), DNS e certificados TLS válidos, simulando um cenário real de infraestrutura web.

---

## Domínio
- **Domínio:** nerdlandia.me  
- **Servidor:** Azure VM (Ubuntu Server)

---

## Serviços Publicados

| Serviço   | Subdomínio                             | Porta Interna |
|----------|----------------------------------------|---------------|
| Nextcloud | https://nextcloud.nerdlandia.me        | 80            |
| Jellyfin  | https://jellyfin.nerdlandia.me         | 8096          |
| Dashy     | https://dashy.nerdlandia.me            | 8080          |

---

## Descrição dos Serviços

### Nextcloud
Nextcloud é uma plataforma de armazenamento e colaboração em nuvem, permitindo upload, sincronização e compartilhamento de arquivos via navegador.

- Serviço autônomo em container Docker  
- Interface web acessível via navegador  
- Utiliza banco SQLite interno (ambiente acadêmico)  
- Acesso HTTPS via SWAG (proxy reverso)  

**Persistência de dados:**
- `./config` – dados e configurações do Nextcloud  

---

### Jellyfin
Jellyfin é um servidor de mídia open source utilizado para gerenciamento e streaming de conteúdos multimídia.

- Serviço autônomo  
- Interface web via navegador  
- Porta interna 8096  
- Tráfego externo roteado pelo SWAG via HTTPS  

**Persistência de dados:**
- `./config` – configurações  
- `./media` – arquivos de mídia  

---

### Dashy
Dashy é um dashboard web auto-hospedado utilizado para centralizar o acesso aos serviços da infraestrutura.

- Serviço autônomo em Docker  
- Interface web acessível via navegador  
- Porta interna 8080  
- Acesso HTTPS através do SWAG  

**Persistência de dados:**
- `./config` – configurações do dashboard  

---

## Estrutura da Aplicação

![Estrutura da Aplicação](https://github.com/user-attachments/assets/149b8f33-be7a-4b87-917b-5eea00858845)

---

## Arquitetura da Aplicação

![WhatsApp Image 2025-12-19 at 15 28 54](https://github.com/user-attachments/assets/2f4c241c-1e46-4eb8-bb2a-072c2862ae4b)


---

## Execução

```bash```
## 👥 Colaboradores
<table>
  <tr>
    <td align="center">
      <a href="https://github.com/LaianeBarreto">
        <img src="https://github.com/LaianeBarreto.png" width="100px;"><br>
        <sub><b>Laiane Barreto</b></sub>
      </a>
    </td>
    <td align="center">
      <a href="https://github.com/robertoferreira7">
        <img src="https://github.com/robertoferreira7.png" width="100px;"><br>
        <sub><b>Roberto Ferreira</b></sub>
      </a>
    </td>
    <td align="center">
      <a href="http://github.com/SamyraFigueredo">
        <img src="https://github.com/SamyraFigueredo.png" width="100px;"><br>
        <sub><b>Samyra Figueredo</b></sub>
      </a>
    </td>
  </tr>
</table>

