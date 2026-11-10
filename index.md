---
title: Política de Privacidade do Pass50+
lang: pt-BR
---

# Política de Privacidade do Pass50+

Última atualização: 9 de novembro de 2026

O Pass50+ é um cofre de senhas. Esta política explica quais dados o aplicativo usa, onde eles ficam e quem pode vê-los. Ela vale para as versões de Android e iPhone.

**Resumo:** suas senhas ficam no seu celular, criptografadas. O desenvolvedor do Pass50+ não tem servidores, não recebe suas senhas e não coleta nenhum dado seu. Não há anúncios, rastreamento nem análise de uso.

## 1. O que você guarda no aplicativo

Nomes de contas, usuários, senhas, sites e observações que você digita ficam num arquivo do cofre, no armazenamento privado do aplicativo no seu celular. Esse arquivo é criptografado com AES-256-GCM. A chave que abre o cofre é protegida de um destes jeitos:

- **Com senha mestra:** a chave é derivada da sua senha mestra com Argon2id. A senha mestra nunca é gravada nem enviada.
- **Sem senha mestra (só Android):** a chave fica guardada no Google Block Store da sua conta Google, criptografada de ponta a ponta pelo Google, e numa área do celular que só abre com o seu rosto, a sua digital, o seu PIN ou o seu padrão.

O desenvolvedor não tem acesso a esse arquivo, à senha mestra nem à chave.

## 2. Quando algum dado sai do celular

Só nas situações abaixo, e sempre para contas ou lugares que são seus:

- **Cópia automática na nuvem.**
  - No Android, o arquivo do cofre, já criptografado, é enviado para uma área privada do aplicativo no seu Google Drive. Essa área não aparece nos seus arquivos e só o Pass50+ a acessa.
  - No iPhone, quando essa opção existe, o arquivo vai para o seu iCloud.
  - A senha mestra e o código do Kit de Emergência nunca são enviados.
- **Login com a conta Google (Android).** Serve para acessar a área privada do Drive. O Google informa ao aplicativo o seu e-mail e o seu nome. O Pass50+ não guarda nem envia esses dados a ninguém.
- **Chave do cofre sem senha mestra (Android).** Fica no Google Block Store da sua conta, para que um celular novo restaurado do seu backup do Google consiga abrir o cofre. Sem bloqueio de tela no celular, a chave não é enviada à conta e fica só no aparelho.
- **Cópia em arquivo e Kit de Emergência.** Vão para o lugar que você escolher: a pasta do celular, um pendrive, o Drive ou outro aplicativo. A partir daí, quem cuida do arquivo é você e o serviço escolhido.
- **Preenchimento automático (Android).** Ao conferir se um aplicativo pertence ao site de uma senha, o celular consulta o endereço público `/.well-known/assetlinks.json` desse site. O site fica sabendo que o seu aparelho fez a consulta, como acontece ao abrir qualquer página. Nenhuma senha é enviada nessa consulta.

O backup automático do Android fica desligado para o Pass50+, e o arquivo do cofre não passa para outro celular na transferência entre aparelhos. No iPhone, o backup do aparelho (iCloud ou computador) inclui o arquivo do cofre, que continua criptografado.

## 3. Preenchimento automático (Android)

Se você ligar o Pass50+ como serviço de preenchimento nos ajustes do celular, o Android mostra ao aplicativo a estrutura da tela de outros aplicativos e sites quando um campo de login aparece. O Pass50+ usa isso só para achar os campos de usuário e senha e descobrir qual site ou aplicativo está pedindo a senha. Tudo é feito no celular, e nada disso é guardado ou enviado.

Para o preenchimento funcionar com o cofre trancado, o Pass50+ guarda uma cópia separada das senhas no celular. Os usuários e as senhas dessa cópia são criptografados com uma chave do próprio Android:
- no cofre com senha mestra, só o seu rosto ou a sua digital abrem essa chave;
- no cofre sem senha mestra, o PIN e o padrão também valem.

Desligar o preenchimento nos Ajustes do Pass50+ apaga essa cópia.

## 4. Outros recursos do celular

- **Rosto e digital.** Quem confere é o próprio celular. O Pass50+ nunca recebe nem guarda dados biométricos.
- **Área de transferência.** Uma senha copiada é apagada sozinha depois de 30 segundos.
- **Ouvir letra por letra.** Usa a voz do próprio celular. No Android, o aplicativo escolhe só vozes geradas no aparelho, para a senha soletrada não sair dele.
- **Capturas de tela.** São bloqueadas nas telas do aplicativo.

## 5. Permissões

Internet, para a cópia na nuvem e a conferência de sites; biometria, para o rosto e a digital; vibração; e detecção de captura de tela. O aplicativo não pede acesso a fotos, contatos, localização, câmera ou microfone.

## 6. Como apagar seus dados

- **No celular:** desinstalar o aplicativo apaga o cofre, as preferências e a cópia do preenchimento.
- **No Google Drive:** abra o Google Drive no navegador, vá em Configurações → Gerenciar apps e use "Excluir dados ocultos do app" no Pass50+.
- **No Google Block Store:** a chave do cofre sem senha mestra é apagada quando o cofre passa a usar senha mestra. Ela também pode permanecer no backup do seu celular na conta Google, de onde sai ao apagar esse backup nas configurações da conta.
- **No iCloud:** em Ajustes do iPhone → seu nome → iCloud → Gerenciar Armazenamento, apague os dados do Pass50+.

Como o desenvolvedor não recebe dados seus, não há nada a apagar do lado dele.

## 7. Crianças

O Pass50+ não é voltado a crianças e não coleta dados de ninguém, inclusive de menores.

## 8. Seus direitos (LGPD)

O desenvolvedor não coleta nem trata dados pessoais dos usuários: tudo o que você guarda fica no seu celular e nas suas contas. Os dados enviados ao Google ou à Apple seguem as políticas de privacidade dessas empresas. Para dúvidas sobre esta política, fale com o desenvolvedor pelo contato abaixo.

## 9. Mudanças nesta política

Se esta política mudar, a nova versão será publicada neste endereço, com a data de atualização no topo.

## Contato

Abel Angelo  
abelangelodev@gmail.com
