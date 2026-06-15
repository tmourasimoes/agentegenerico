---
trigger: always_on
---

## DEPLOY

# Regras de Deploy

Sempre perguntar o nome do projeto, a pasta aonde será feito o deploy. Armazenar a informação para cada prodjeto.
No final confirmar as informações antes de fazer o deploy.


## Instruções Adicionais

- Antes de iniciar a cópia, limpe e recrie o diretório informado.
- Sempre use caminhos relativos ao `projectRoot` do script de deploy (`build_deploy.js`).
- Ao final do empacotamento, gere os instaladores automatizados `install.bat` e `uninstall.bat` e 'update.bat' na raiz do diretório informado.

install.bat - instala todos os pré-requisitos para sistema funcionar.
update.bat - instala, somente as atualizações de sistema, banco de dados se houver não atualizar.
uninstall.bat - Perguntar se quer desinstalar o banco de dados, os sistemas de pré - requisito. e desisntala todos os sistemas que foram instalados e inclusive a pasta .

