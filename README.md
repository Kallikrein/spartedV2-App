# spartedV2-App


### Initialization  
Repository was initialised with the following parameters :

```
docker pull kallikrein/android-sdk
```  
```
alias drun='docker run -it --rm'
alias mine='sudo chown -R $USER'
alias npm='drun -v $PWD:/src kallikrein/sails-tools npm'
alias sails='drun -v $PWD:/src kallikrein/sails-tools sails'
alias lift='drun -v $PWD:/src -p 80:1337 kallikrein/sails-tools sails lift'
alias nodemon='drun -v $PWD:/src -p 80:1337 kallikrein/sails-tools nodemon'
alias bower='drun -v $PWD:/src -p 80:1337 kallikrein/sails-tools bower --allow-root '
alias cordova='drun --privileged -v /dev/bus/usb:/dev/bus/usb -v $PWD:/src -v $PWD/gradle:/root/.gradle kallikrein/android-sdk cordova'
alias adb='drun --privileged -v /dev/bus/usb:/dev/bus/usb -v $PWD:/src kallikrein/android-sdk adb'
```

### Build
```
cordova create sparted com.sparted sparted
```  
```
mine sparted
```  
```
cd sparted
```  
```
cordova platform add android
```  
```
cordova run
```  