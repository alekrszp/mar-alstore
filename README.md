## Iniciar o projeto (passo a passo)

- **Pré-requisitos:** Node (recomendado >=16), `npm` ou `yarn`. Opcional: Android Studio (emulador) ou Xcode (macOS). Para testar em dispositivo físico, instale o app Expo Go no celular.

- **Criar o projeto (uma vez):**

```powershell
# criar na pasta atual (cuidado: não sobrescrever arquivos existentes)
npx create-expo-app . --template blank

# ou criar em uma nova pasta
npx create-expo-app nome-do-app --template blank
cd nome-do-app
npm install
```

- **Rotina diária — comandos que você deve executar sempre que iniciar o trabalho:**

```powershell
# 1) entrar na pasta do projeto
cd marcal

# 2) instalar dependências (faça sempre que clonar o repo ou quando package.json mudar)
npm install

# 3) iniciar o servidor de desenvolvimento (Metro)
npx expo start
```

- **Opções úteis ao iniciar:**
	- Limpar cache: `npx expo start -c`
	- Forçar túnel (útil em redes restritas): `npx expo start --tunnel`
	- Abrir no emulador Android (Windows/Linux): `npx expo start --android` ou, após `npx expo start`, pressione `a`.
	- Abrir no iOS simulator (macOS): `npx expo start --ios` ou, após `npx expo start`, pressione `i`.
	- Abrir no navegador (web): `npx expo start --web`

- **Executar em dispositivo físico:** abra o Expo Go no celular e escaneie o QR code exibido pelo `npx expo start`.

- **Comandos úteis adicionais:**
	- Parar o servidor: Ctrl+C
	- Adicionar dependência: `npm install <pacote>` ou `yarn add <pacote>`
	- Remover `node_modules` e reinstalar rapidamente: PowerShell: `Remove-Item -Recurse -Force node_modules; npm install`

- **Dicas rápidas:**
	- Se algo travar, tente `npx expo start -c`.
	- Mantenha Node e Expo atualizados para evitar incompatibilidades.