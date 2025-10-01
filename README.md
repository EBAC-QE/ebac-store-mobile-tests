# 📱 Instalar o app EBACShop no emulador Android

## ✅ Pré-requisitos
Antes de começar, verifique se você tem os seguintes itens instalados e configurados no seu ambiente:

- [Java JDK 11+](https://www.oracle.com/java/technologies/javase/jdk11-archive-downloads.html)  
- [Android Studio](https://developer.android.com/studio) (com o **Android Emulator** configurado)  
- [Bundletool](https://developer.android.com/studio/command-line/bundletool) baixado e disponível no PATH  

> Para confirmar, rode no terminal:  
> ```bash
> java -version
> bundletool version
> ```

---

## 1. Baixar o pacote de APKs
Baixe o arquivo `.apks.zip` neste link:  
👉 [Download ebacshop.apks.zip](https://github.com/EBAC-QE/ebac-store-mobile-tests/raw/apks/app/ebacshop.apks.zip)

Após o download, extraia o arquivo para obter o **`ebacshop.apks`**.

---

## 2. Abrir o emulador Android
Abra o **Android Emulator** no Android Studio (ou outro emulador configurado).  
Deixe o emulador rodando, pois o **bundletool** vai instalar o app diretamente nele.

---

## 3. Instalar com o bundletool
No terminal, vá até a pasta onde está o arquivo **`ebacshop.apks`** e execute:

```bash
bundletool install-apks --apks=./ebacshop.apks
```

## 4. Confirmar a instalação

Após a execução, o app EBACShop estará disponível no emulador, pronto para ser aberto e testado

