📝 Descrição

Este projeto consiste em um Keylogger desenvolvido em Python para fins estritamente educacionais. Ele foi criado como parte de um laboratório prático para entender como malwares de monitoramento capturam entradas de teclado e realizam a exfiltração de dados via protocolo SMTP (e-mail).

O script captura as teclas pressionadas, formata caracteres especiais (como Espaço, Enter e Backspace) e envia relatórios periódicos para um e-mail configurado a cada 60 segundos.

🛠️ Tecnologias e Bibliotecas
Python 3.13+
Pynput: Utilizada para monitorar eventos de entrada (teclado).
Smtplib: Biblioteca padrão para envio de e-mails usando o protocolo SMTP.
Threading: Para gerenciar o envio automático em segundo plano sem interromper a captura.
MIMEText: Para estruturar o conteúdo do e-mail.
🚀 Funcionalidades

Captura de teclas alfanuméricas em tempo real.

Tratamento de teclas especiais (Enter, Tab, Backspace, Espaço).

Envio automatizado de logs por e-mail (Gmail SMTP).

Sistema de persistência de log: caso o envio falhe, o log é mantido para a próxima tentativa.

Tratamento de exceções para teclas de sistema (teclas sem caractere).
⚠️ Aviso Legal
Este software foi desenvolvido apenas para fins de aprendizado em segurança da informação. O uso desta ferramenta contra computadores sem autorização prévia é ilegal e constitui um crime cibernético. O autor não se responsabiliza pelo uso indevido deste código.

🛡️ Como se prevenir contra Keyloggers
Entender como o ataque funciona é o primeiro passo para a defesa. Aqui estão as principais medidas de mitigação:

1. Uso de Antivírus e EDR
Softwares de proteção modernos (como Windows Defender ou soluções corporativas de EDR) conseguem detectar o comportamento do pynput ou scripts Python não assinados que tentam monitorar o teclado, bloqueando-os antes da execução.

2. Autenticação de Dois Fatores (2FA)
Mesmo que um atacante capture sua senha através de um keylogger, o 2FA (via aplicativo ou chave física) impede o acesso à conta, pois o código dinâmico não pode ser previsto pelo malware.

3. Teclados Virtuais em Sites Sensíveis
Para operações bancárias, muitos sites oferecem teclados virtuais onde o clique do mouse substitui a digitação. Isso evita que o keylogger capture a sequência de teclas.

4. Gestores de Senhas
O uso de gestores de senhas (como Bitwarden ou 1Password) permite o preenchimento automático das credenciais. Como você não digita a senha caractere por caractere, o keylogger não consegue capturar a informação.

5. Higiene Digital
Evite baixar arquivos de fontes desconhecidas.
Não execute scripts ou programas .exe enviados por e-mails suspeitos (Phishing).
Mantenha o sistema operacional e os navegadores sempre atualizados.

