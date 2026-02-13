# Linux Tails Portátil
Configuração pessoal e notas operacionais para um ambiente de segurança amnésico em um pendrive.

[**EN-US**](../README.md)

<img width="1599" height="899" alt="image" src="https://github.com/user-attachments/assets/8e0b2aeb-3730-4041-ae25-bdacdf6ff8db" />


## Dependências
- [Tails OS](https://tails.net/install/download/index.en.html)

## Primeiros Passos
<details>
  <summary>Iniciando o Linux Tails</summary>

  - Conecte o pendrive e reinicie o seu sistema.
  - Pressione **F12** (ou a tecla específica do seu hardware) durante a inicialização para abrir o Menu de Boot.
  - Selecione a partição **UEFI** do pendrive.
  - Na tela `Welcome to Tails`, navegue até `Additional Settings` (ícone de +) e defina uma **Senha de Administração** se o acesso root (sudo) for necessário.
</details>

<details>
  <summary>Conectar à rede Tor</summary>
  
  - Na página `Tor Connection Assistant`, selecione a opção **"Hide to my local network that I'm connecting to Tor"** para maior ofuscação.
  - [Solicite uma ponte](https://bridges.torproject.org/options) e insira as credenciais manualmente ou via código QR.
  - Certifique-se de que o horário do sistema esteja sincronizado com o **UTC**. Se a conexão falhar, pode ser necessário ajustar o **Relógio da BIOS/Hardware** para o UTC para permitir o handshake do Tor.
</details>

## Recomendações de Segurança
  - **Mantenha o SO Atualizado**: Sempre atualize para a versão estável mais recente assim que estiver disponível. Versões desatualizadas podem conter vulnerabilidades ou protocolos de ponte obsoletos que comprometem sua segurança.
  - **Sem Armazenamento Persistente**: Não crie uma partição persistente. Isso garante que nenhum dado de sessão, arquivos baixados ou configurações sejam salvos no hardware físico, não deixando nenhum rastro após o desligamento.
  - **Nunca Maximize o Tor Browser**: Mantenha sempre o Tor Browser no tamanho de janela padrão. Uma janela maximizada expõe a resolução da sua tela, o que pode ser usado para identificar e rastrear você entre sessões.
  - **Sempre Use Teclado e Idioma em Inglês**: Mantenha o idioma do sistema e o layout do teclado configurados em inglês. Configurações em outros idiomas podem revelar sua localidade e reduzir o anonimato, tornando sua sessão distinguível da maioria dos usuários do Tor.
