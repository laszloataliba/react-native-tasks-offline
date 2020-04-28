# react-native-tasks-offline
Desenvolvimento do App tasks(offline)

(no diretório raiz) react-native init "Nome-App"(=Nome-diretório a ser criado)

(no diretório raiz) emulator -list-avds
(no diretório raiz) emulator -no-snapshot -avd "Nome-Emulador"

(no diretório criado) react-native run-android


Criando nova branch para a aplicação react-native

- Baixar os arquivos da branch selecionada(Master, provavelmente);
- criar a branch(git checkout -b "Nova Branch") nova imediatamente após download da "Master";
- Caso ocorra o erro abaixo ao executar o comando react-native run-android:

react-native run-android: error Android project not found. Are you sure this is a React Native project? 
If your Android files are located in a non-standard location (e.g. not inside 'android' folder), consider setting `project.android.sourceDir` option to point to a new location. 
Run CLI with --verbose flag for more details.

Solution 1 :

1. Open your React Native Project Root Directory and locate android -> app -> build -> intermediates -> signing_config -> debug -> out -> signing-config.json.

2. Delete the signing-config.json file and then again GoTo your react native project root directory and run again project using react-native run-android command.  

3. Execute emulator -no-snapshot -avd "Nome_Emulador".

4. Abra outro terminal e execute react-native run-android.

