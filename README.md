<img width="2878" height="1718" alt="adb" src="https://github.com/user-attachments/assets/e5751ea5-2e0d-4e34-be67-de190b625295" />
<img width="969" height="1594" alt="Définir 3 scénarios simples" src="https://github.com/user-attachments/assets/3faa476a-fdc8-4a0b-a499-561269e3d42d" />
<img width="1228" height="547" alt="Démarrer un AVD propre" src="https://github.com/user-attachments/assets/50524caa-0006-4c95-afce-cf797aa3e3ee" />
<img width="1786" height="761" alt="etape 14" src="https://github.com/user-attachments/assets/cacd8ae9-f244-46ee-9c0c-922a7c932652" />
<img width="1170" height="453" alt="Fiche périmètre" src="https://github.com/user-attachments/assets/4d4a08b0-8444-4a74-af3e-0731becb7082" />
<img width="1135" height="434" alt="Installer et lancer l&#39;app de test" src="https://github.com/user-attachments/assets/cb8c4f18-8b2f-4148-b44d-5b35ffc73caa" />
<img width="2073" height="934" alt="logcate" src="https://github.com/user-attachments/assets/74974f95-0ef5-48eb-9617-29a6e07e51d8" />
<img width="1232" height="103" alt="resltat getprop etape 15" src="https://github.com/user-attachments/assets/1e0e9a52-babc-4070-ab3c-3d76faf2fa3c" />
<img width="647" height="327" alt="resultat adb root remount" src="https://github.com/user-attachments/assets/76934471-73bd-485b-a2a2-67f142d13df9" />
<img width="633" height="236" alt="wipe data " src="https://github.com/user-attachments/assets/4b0e9f80-e702-4af6-89d1-f449f3aca13a" />
[lab2.txt](https://github.com/user-attachments/files/25744117/lab2.txt)

<img width="857" height="1242" alt="remise a zero" src="https://github.com/user-attachments/assets/449edd31-7134-47e8-93d6-ea578e661585" />

**Date / Auteur**
04/03/2026 / [HMICH mohammed-amine]

**Support (AVD / device labo)**
AVD – Pixel 6 (émulateur Android)

**Version Android / API**
Android 15 / API level 36

**App + version**
myApplication "2:48" – version 1.0

**3 scénarios**
1.  **Scénario nominal** : Saisie d'un nom et d'un prénom valides, puis envoi du formulaire.
2.  **Scénario de champ vide** : Tentative d'envoi du formulaire sans avoir saisi le prénom.
3.  **Scénario de validation** : Saisie de caractères spéciaux ou chiffres dans les champs "Nom" et "Prénom".

**Observations factuelles**
1.  Après avoir saisi "Dupont" dans le champ "Nom" et "Jean" dans le champ "Prénom", l'appui sur le bouton "Envoyer" ne produit aucun retour visuel ou message de confirmation. On ne sait pas si les données ont été envoyées ou traitées.
2.  Lorsqu'on tente d'envoyer le formulaire avec le champ "Prénom" vide, l'application ne bloque pas l'envoi et ne signale pas l'erreur à l'utilisateur. Le bouton est cliquable et aucun message d'erreur ne s'affiche.
3.  En saisissant "Dupont123" dans le champ "Nom", l'application accepte la saisie sans la filtrer. On ne sait pas si le backend attend un format spécifique (uniquement des lettres).

**Limites**
- Émulateur limité à 4 cœurs CPU et 2 Go RAM
- Google Play Services non disponible
- Matériel simulé (accéléromètre, caméra, GPS, etc.) – comportement potentiellement différent d'un appareil physique
- Pas de carte SD physique

**Reset effectué (Oui/Non) + preuve**
Oui – L'AVD a été remis à son état initial ("wipe data") avant l'exécution des tests.
(Preuve : [Capture d'écran du démarrage de l'AVD avec l'écran d'accueil vierge])

**Propriétés AVD**
avd.ini.displayname              Pixel 6
avd.ini.encoding                 UTF-8
AvdId                            Pixel_6
disk.dataPartition.size          6G
fastboot.chosenSnapshotFile      
fastboot.forceChosenSnapshotBoot no
fastboot.forceColdBoot           no
fastboot.forceFastBoot           yes
hw.accelerometer                 yes
hw.arc                           false
hw.audioInput                    yes
hw.battery                       yes
hw.camera.back                   virtualscene
hw.camera.front                  emulated
hw.cpu.ncore                     4
hw.device.hash2                  MD5:2016577e1656e8e7c2adb0fac972beea
hw.device.manufacturer           Google
hw.device.name                   pixel_6
hw.dPad                          no
hw.gps                           yes
hw.gpu.enabled                   yes
hw.gpu.mode                      auto
hw.gyroscope                     yes
hw.initialOrientation            portrait
hw.keyboard                      yes
hw.lcd.density                   420
hw.lcd.height                    2400
hw.lcd.width                     1080
hw.mainKeys                      no
hw.ramSize                       2048
hw.sdCard                        yes
hw.sensors.light                 yes
hw.sensors.magnetic_field        yes
hw.sensors.orientation           yes
hw.sensors.pressure              yes
hw.sensors.proximity             yes
hw.trackBall                     no
image.sysdir.1                   system-images\android-36\google_apis\x86_64\
PlayStore.enabled                false
runtime.network.latency          none
runtime.network.speed            full
showDeviceFrame                  yes
skin.dynamic                     yes
tag.display                      Google APIs
tag.displaynames                 Google APIs
tag.id                           google_apis
tag.ids                          google_apis
target                           android-36
vm.heapSize                      228
