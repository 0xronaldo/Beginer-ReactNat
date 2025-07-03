

### Primeros Pasos en ReactNat-v0.79

primero instalamos con : 
```
npm uninstall -g react-native-cli @react-native-community/cli
```

Luego se inicializa el proyecto de la siguiente manera 

```
npx @react-native-community/cli@latest init AwesomeProject
```


## configuraciones con Java 17^ -> recomendado jdk21

configuracion en ArchLinux 

```

$ sudo pacman -S jre21-openjdk 
$ sudo pacman -S jdk21-openjdk

```
## ejecucion combinada (opcional) -> depende de la distribucion

```
$ archlinux-java set java-(version)-openjdk

  comando opcional para ver el estado <br>

$ archlinux-java get 

```
### Configuracion de JAVA_HOME

Configuracion en BASH ( "~/.bashrc" ) 

```

' source JAVA_HOME="/usr/lib/jvm/java-21-openjdk" '
' source PATH="$JAVA_HOME"/bin:$PATH" '

```

Configuracion en ZSH ( " ~/.zshrc" )

```
'export JAVA_HOME="/usr/lib/jvm/java-21-openjdk"'
'export PATH="$JAVA_HOME"/bin:$PATH"'

```

## Configuracion para Android Studio 

primero descargar el paquete de Android Studio de su pagina oficial 

<p><span>Enlace: <a> https://developer.android.com/studio?hl=es-419 </a> </span>

despues de haber instalado se tiene la configuracion de ANDROID_HOME

se configura los sdk_manager | es necesario que se tenga configura | las versiones de SDK de android (12) - (15)

### Configuracion del PATH para ANDROID_HOME 

configuracion del path

Configuracion en BASH ( "~/.bashrc" ) 

```

export ANDROID_HOME=$HOME/Android/Sdk
export PATH=$PATH:$ANDROID_HOME/emulator
export PATH=$PATH:$ANDROID_HOME/platform-tools

```

Configuracion en ZSH ( " ~/.zshrc" )

```
export ANDROID_HOME=$HOME/Android/Sdk
export PATH=$PATH:$ANDROID_HOME/emulator
export PATH=$PATH:$ANDROID_HOME/platform-tools
```


### Ejecucion de React Native

primero 

```
npx @react-native-community/cli@latest init AwesomeProject --version 0.XX.X

```
en una terminal diferente ejecutar metro 

cd AwensomeProject 
```
$ npm start 
```

en otra terminal ejecutar ReactNative

```
$ npm run android 

```



