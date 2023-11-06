# Laboratório Ransomware:

*	Criar uma VM no Virtual Box, Proxmox, VirtManager ou Hyper-V sem placa de rede (opcional, download de uma imagem pronta para importar no VirtualBox ou converter https://github.com/ivandroconradi/winxpimage)
*	Criar um snapshot
*	Fazer o download do [KMS Pico](https://github.com/zbezj/HEU_KMS_Activator/releases/tag/41.2.0), das amostras dos [Ransonware](https://github.com/ivandroconradi/lab_ransomware/new/main?readme=1#malwares) e descompactar com a senha “infected”
*	Depois da instalação ou importação do Windows, verificar novamente se a VM está sem placa de rede e isolada
*	Criar um novo snapshot
* Analisar e corrigir caso necessário o registro do Windows com o Ccleaner
*	Instalar o KMS e verificar as alterações feitas no registro do Windows
*	Com o programa Network Traffic View, visualizar as tentativas de comunicação com a internet durante a execução do KMS
*	Analisar o registro do Windows com o Ccleaner novamente
*	Executar e acompanhar as novas mudanças no regedit e o que o ransomware tentou comunicar na internet
*	Voltar o snapshot, instalar o BitDefender e realizar novamente os testes. Depois pode instalar outros antivírus para analisar. Teste o antivírus com a opção contra ransomware desativada e também com ela ativada para observar a reação.
*	Melhorar esta lista de testes com mais sugestões 


# Ferramentas Uteis:

#### O Process Monitor é uma ferramenta de monitoramento avançada para Windows que mostra em tempo real o sistema de arquivos, o Registro e a atividade do processo/thread.
https://learn.microsoft.com/pt-br/sysinternals/downloads/procmon


#### O Autouns tem o conhecimento mais abrangente dos locais de inicialização automática de qualquer monitor de inicialização, mostra quais programas estão configurados para serem executados durante a inicialização ou logon do sistema.
https://learn.microsoft.com/pt-br/sysinternals/downloads/autoruns


#### O ListDLLs é um utilitário que informa as DLLs carregadas em processos. Você pode usá-lo para listar todas as DLLs carregadas em todos os processos, em um processo específico ou para listar os processos que têm uma DLL específica carregada.
https://learn.microsoft.com/pt-br/sysinternals/downloads/listdlls

#### O DiskMon é um aplicativo que registra e exibe todas as atividades do disco rígido em um sistema Windows.
https://learn.microsoft.com/pt-br/sysinternals/downloads/diskmon

#### Gerenciador de Processos mostra informações sobre quais identificadores e processos de DLLs foram abertos ou carregados.
https://learn.microsoft.com/pt-br/sysinternals/downloads/process-explorer

#### Compara as subchaves ou entradas do registro especificadas.
https://learn.microsoft.com/pt-br/windows-server/administration/windows-commands/reg-compare

#### Compara o registro do Windows antes e depois de uma alteração
https://sourceforge.net/projects/regshot/

#### O RegistryChangesView é uma pequena ferramenta gratuita que lhe permite monitorar e detectar alterações no registro do Windows.
http://www.nirsoft.net/utils/
http://www.nirsoft.net/utils/registrychangesview-x64.zip

https://learn.microsoft.com/pt-br/windows-server/administration/windows-commands/fc

#### Network Traffic View é um aplicativo que serve, basicamente, para monitorar a sua rede de computadores.
http://www.nirsoft.net/utils/network_traffic_view.html


# Malwares

#### https://github.com/ivandroconradi/theZoo/tree/master/malware/Binaries/Ransomware.Cryptowall

As principais formas de contaminação do cryptowall por fraude são:

```
Aviso de faturas;
Pedidos de compra;
Reclamações de clientes;
Cliques em anúncios fraudulentos;
Demais comunicações de negócios.
```

Normalmente os arquivos maliciosos de cryptowall são instalados nos % ou %temp% ou então em pastas % AppData.

A partir do momento em que a infecção é realizada, o malware irá analisar todas as informações disponíveis no disco rígido e realizará a criptografia das informações.

O cryptowall também vasculha as unidades removíveis, podendo inutilizar pen drives, cartões de memória e HDs externos que estejam conectados à máquina. Ele pode infectar todas as unidades de rede mapeadas como uma letra de unidade na máquina infectada.



#### https://github.com/ivandroconradi/theZoo/tree/master/malware/Binaries/Ransomware.Locky

Locky é um tipo de ransomware utilizado em ataques de 2016, por todo o mundo. Ele tem a capacidade de criptografar mais de 160 tipos de arquivos, e é instalado ao enganar as vítimas, que acreditam estar abrindo e-mails íntegros, mas que, na verdade, são criminosos. Seus anexos, com ransomware, são de um método denominado phishing.



#### https://github.com/ivandroconradi/theZoo/tree/master/malware/Binaries/Ransomware.Jigsaw

O Jigsaw ameaça excluir arquivos caso o resgate não seja pago dentro de um período estabelecido.
Diferente de outros ransomware, o Jigsaw impede que a vítima reinicie o computador ao ser infectado, ameaçando excluir os arquivos caso a pessoa faça essa operação.



#### https://github.com/ivandroconradi/theZoo/tree/master/malware/Binaries/Ransomware.Petya

O Petya atinge sistemas inteiros de computador, criptografando todo o disco rígido da vítima, de forma semelhante ao GoldenEye; porém, atingindo o Master Boot Records. Ao sofrer o ataque, a vítima encontra, em sua tela inicial, o desenho de uma caveira com dois ossos cruzados.

É muito comum que esse tipo de ransomware se espalhe pelos departamentos de RH, a partir de e-mails falsos de solicitação de emprego, geralmente com um link infectado para o portfólio do suposto candidato.




### Security Report
https://www.securityreport.com.br/email/InfoSR2023.html

### Reportando amostras:
https://www.virustotal.com/gui/

https://id-ransomware.malwarehunterteam.com/index.php?lang=pt_PT

https://support.avast.com/pt-br/article/threat-lab-report-malware/#pc



### Keylogger
https://github.com/ivandroconradi/theZoo/tree/master/malware/Binaries/Keylogger.Ardamax



