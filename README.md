## TInject-corporate-v2<br></br>

﻿# Componente TInject Corporate
Componente para criação de chatBots com delphi<br>
<i>Component for creating chatBots with delphi</i><br></br>

## INSTRUÇÕES PARA USO DO COMPONENTE<br></br>

Compatibilidade testada nas seguintes versões do Delphi: Seattle, Berlim, Tokyo, Rio, Sydney, Athens, Alexandria, Florence.<br></br>

### Para contratação da licença do Corporate entre em contato no whatsApp:(81) 99630-2385<br>

Instruções básicas para instalação:<br></br>

1. Desinstale completamente o CEF e os arquivos .bpl na pasta da Embarcadero<br>
2. Renomeie qualquer pasta de versões anteriores do CEF<br> 
3. Desinstale completamente o Tinject Corporate<br>
4. Renomeie qualquer pasta de versões anteriores do Tinject Corporate<br>
5. Remova todos os diretorios antigos do CEF e do Tinject Corporate do Library path do seu Delphi<br>
6. Incluir todos os diretorios da nova versão do CEF e do Tinject Corporate V2<br>
7. Instale o CEF<br>
8. Instale o Tinject Corporate V2<br>
9. Extraia os arquivos binários(CEF4BIN_154.0.32.rar) para a basta BIN do demo<br>
10. Coloque o seu serial(Token) na propriedade serialCorporate e rode e demo<br>

### Tutorial de instalação padão:<br>
https://www.youtube.com/watch?v=EIxFdtenNxI&t=31s
<br>
### Tutorial de instalação manual Delphi Alexandria e Florence:<br>
https://www.youtube.com/watch?v=mifdSA-Hkyk

<br>
Videos demo:
<br>
https://youtu.be/YEmwghSGoFA
<br>
https://youtu.be/07RoReOHaT4
<br>
https://youtu.be/cbWW7VNYwEo
<br><br>

### Recursos / Resources<br><br>
✔️  Login<br>
✔️  Logout<br>
✔️  Confirmação de entrega de mensagens - Message delivery confirmation<br>
✔️  Enviar mensagens de texto com botão e lista - Send text message with button and list<br>
✔️  Enviar mensagens de texto para números fora da agenda - Send text message<br>
✔️  Enviar mensagens para grupos - Send group messages<br>
✔️  Enviar contatos - Send phone contacts<br>
✔️  Rejeitar ligações - Reject calls<br>
✔️  Enviar chave PIX<br>
✔️  Enviar MP3 - Send MP3<br>
✔️  Enviar MP4 - Send MP4<br>
✔️  Enviar IMG - Send IMG<br>
✔️  Enviar RAR - Send RAR<br>
✔️  Enviar Link com prévia - Sending and preview (Não compatível com o multi device)<br>
✔️  Enviar localização - Location sending<br>
✔️  Enviar Stickers - Send Stickers<br>
✔️  Listar contatos - Contact list<br>
✔️  Listar bate papos - Conversation list<br>
✔️  Simular digitando - Typing simulation<br>
✔️  Recebimento de novas mensagem - Receiving new messages<br>
✔️  Configurações de DDI - International number configuration<br>
✔️  Validação de números - number validator<br>
✔️  Checagem de conexão - check connection<br>
✔️  Download de arquivos - Download files<br>
✔️  Download da foto de perfil - Download profile picture<br>
✔️  Criar grupo - Create group (Não compatível com o multi device)<br>
✔️  Sair do grupo - Leave the group (Não compatível com o multi device)<br>
✔️  Adicionar participante ao grupo - Add participant to the group (Não compatível com o multi device)<br>
✔️  Remover participante do grupo - Remove group member (Não compatível com o multi device)<br>
✔️  Promover participante adminstrador do grupo - Promote participant group administrator (Não compatível com o multi device)<br>
✔️  Despromover participanete adminstrador do grupo - Demote participating group administrator (Não compatível com o multi device)<br>
✔️  Listar todos os grupos - List all groups<br>
✔️  Listar participantes do grupo - List group participants<br>
✔️  Obter link convite de grupos - Get Group invitation link<br>
✔️  Entrar em grupo via link convite - Join group via invitation link<br>
✔️  Monitoramento automático em caso de atualizações disponíveis do WhatsApp - Automatic monitoring in case of available WhatsApp updates<br>

### Cursos do componente / Component lessions:<br>

[Clique aqui / Click where](http://mikelustosa.kpages.online/tinject)

### Official documentation:<br><br>

### Events that send messages<br>
| event           | Description                | Example                                                                              | return |
|-----------------|----------------------------|--------------------------------------------------------------------------------------|--------|
| send            | Send text message          | TInject1.send('55819999999@c.us', 'hello');                                          | onGetIsDelivered |
| sendButtons     | Send text message buttons  | TInject1.sendButtons('55819999999@c.us', 'Choose', [{buttonId: 'id1', buttonText:{displayText: 'SIM'}, type: 1}, type: 1}], 'Escolha uma opção'); | -      |
| sendFile        | Send file and text message | TInject1.SendFile('558199999999@c.us', 'c:\myFile.pdf', 'hello');                    | onGetIsDelivered |
| sendContact     | Send whatsapp contact      | TInject1.sendContact('destinationContact@c.us', 'contactToBeSent@c.us');             | -      |
| sendLinkPreview | Send preview link          | TInject1.sendLinkPreview('558199999999@c.us', 'https://youtube.com/video', 'hello'); | -      |
| sendLocation    | Send Location              | TInject1.sendLocation('55819999999@c.us', '-70.4078', '25.3789', 'my location');     |        |
| sendPixKey      | Send PIX Key               | TInject1.sendPixKey('55819999999@c.us', 'EMAIL or CPF or CNPJ or TELEFONE or ALEATÓRIO', 'Chave PIX', 'NAME');                    |        |
| sendStartTyping | Send start typing          | TInject1.sendStartTyping('55819999999@c.us');                                        |        |
| sendStopTyping  | Send stop typing           | TInject1.sendStopTyping('55819999999@c.us');                                         |        |
| sendSticker     | Send Stickers              | TInject1.sendSticker('55819999999@c.us', 'Long base64 where...');                    |        |<br><br>

### Verifications events<br>
| event                 | Description                                             | example                                              | event return      | return                       |
|-----------------------|---------------------------------------------------------|------------------------------------------------------|-------------------|------------------------------|
| CheckIsConnected      | Checks the connection between the device and whatsapp   | TInject1.CheckIsConnected();                         | OnIsConnected     | boolean                      |
| NewCheckIsValidNumber | Checks whether one or more numbers are whatsapp numbers | TInject1.NewCheckIsValidNumber('558199999999@c.us'); | OnNewGetNumber    | TReturnCheckNumber           |
