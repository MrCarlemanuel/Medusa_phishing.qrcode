# Medusa_phishing.qrcode

Medusa Phisher é um *script* de ferramenta de *phishing* projetado para criar páginas de *phishing* para vários serviços online. Ele permite que os usuários configurem páginas de *phishing* para serviços como Instagram, Facebook, Twitter e mais. O *script* facilita a hospedagem dessas páginas de *phishing* usando `localhost.run` para tunelamento, tornando fácil a captura de credenciais de usuários.

## 🛑 ISENÇÃO DE RESPONSABILIDADE (DISCLAIMER)

**Este *script* destina-se apenas a fins educacionais e de testes de penetração éticos.**

O uso indevido desta ferramenta para atividades ilegais ou maliciosas é **estritamente proibido** e pode resultar em consequências legais severas. O autor não assume nenhuma responsabilidade por qualquer uso indevido ou dano causado por este *script*. **Use por sua conta e risco e sempre com consentimento explícito do proprietário do sistema.**

## ✨ Funcionalidades (Features)

  * Cria páginas de *phishing* para múltiplos serviços online.
  * Hospeda páginas de *phishing* usando `localhost.run` para fácil acesso.
  * Captura credenciais inseridas nas páginas de *phishing* para análise.
  * O *link* de *phishing* gerado é exibido, juntamente com seu código QR.

## 🛠️ Dependências (Dependencies)

Para o correto funcionamento do script, você precisa:

  * `PHP`: Necessário para hospedar as páginas de *phishing* localmente.
  * `SSH`: Necessário para criar túneis SSH usando `localhost.run`.
  * `XTERM`: Necessário para gerar o link e o código QR.

**(Nota:** O `setup.sh` instala essas dependências para você.)

## 💻 Ambiente Suportado (Supported Environment)

  * Kali Linux
  * Parrot Security OS
  * Debian
  * Ubuntu
  * Arch

-----

## 🚀 Guia de Uso (Passo a Passo)

### 1\. Preparação

1.  Clone o repositório:
    ```bash
    git clone https://github.com/Adrilaw/MedusaPhisher.git
    [WhatsApp Image 2025-10-31 at 23 20 27](https://github.com/user-attachments/assets/447c5875-0b1e-4116-984a-7feae2cbfa0b)

2.  Navegue até o diretório do *script*:
    ```bash
    cd MedusaPhisher
    ```
3.  Conceda permissões de execução aos *scripts*:
    ```bash
    chmod +x medusa_phisher.sh
    chmod +x setup.sh
    ```
4.  Execute a instalação das dependências:
    ```bash
    sudo ./setup.sh
    ```

### 2\. Execução do Script

1.  Execute o *script* principal:

    ```bash
    sudo ./medusa_phisher.sh
    ```

2.  **Selecione o alvo de Phishing:** Escolha a opção desejada no menu (Ex: **Instagram**).

  ![WhatsApp Image 2025-10-31 at 23 05 54](https://github.com/user-attachments/assets/2b7a7484-6ea4-4353-8619-24a2fc630b95)


3.  **Configuração do Tunelamento:** Selecione o método de tunelamento (`localhost.run`) e a porta (padrão 5555).

    O terminal irá iniciar o túnel e gerar as informações de conexão.

![WhatsApp Image 2025-10-31 at 23 05 55](https://github.com/user-attachments/assets/059ea203-ff05-43e2-880d-a899da44fc44)

### 3\. A Página Clonada

O *script* abrirá um terminal *xterm* mostrando o link de *phishing* e o código QR.
A vítima (em um ambiente de teste ético) acessaria o link e veria a página clonada.

![WhatsApp Image 2025-10-31 at 23 05 54 (1)](https://github.com/user-attachments/assets/4e917265-7a50-41aa-bf4c-597bf4b810f2)


### 4\. Captura de Dados

Quando a "vítima" insere as credenciais na página falsa e tenta fazer o *login*, o *script* captura e exibe os dados no seu terminal.
![WhatsApp Image 2025-10-31 at 23 05 55 (1)](https://github.com/user-attachments/assets/1b01855a-796b-419a-90b2-c5fe3348b1c2)
-----

## ✍️ Autor (Author)

Adrilaw @ GitHub
Kidpentester @ xda-developers

## 📄 Licença (License)

MedusaPhisher está licenciado sob a [Licença Pública Geral GNU (GNU General Public License)](/Adrilaw/MedusaPhisher/blob/main/LICENSE) - veja o arquivo `LICENSE` para detalhes.
