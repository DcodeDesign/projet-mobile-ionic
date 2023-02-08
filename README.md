# AppMobile

## Capacitor: Install the native platforms you want to target.
```
npm i @capacitor/ios @capacitor/android
npx cap add android
npx cap add ios
ng build
```

### Sync the build folder to native projects
```
npx cap sync
```

### command to directly open Android Studio or Xcode
```
npx cap open ios
npx cap open android
```

### command to directly open Android Studio or Xcode
```
npx cap run ios
npx cap run android
```

### Capacitor Live Reload
```
ipconfig getifaddr en0


ng serve -o --host localhost
npx cap run android -l --external
npx cap run ios -l --external
```

#### Alternative
```
ng serve -o --host localhost:4200
ng serve -o --host 10.0.2.2:4200

npx cap run android -l --external --host localhost:4200
npx cap run android -l --livereload-url=http://localhost:4200
npx cap run android --livereload-url=http://10.0.2.2:4200
npx cap run android --livereload-url=http://localhost:4200
npx cap run ios --livereload-url=http://localhost:4200
npx cap run android -l --host=localhost --port=4200
npx cap run ios -l --external


ionic cap add android
ionic cap sync
ionic cap build android
ionic cap run android --external -livereload
```

## Other command
```
npx cap doctor
ionic info

rm -rf node_modules package-lock.json
npm cache clean -f

sudo npm install -g @ionic/app-scripts@latest --save-dev
npm install --python=python2.7 
npm config set python python2.7
npm install node-sass@6.0 
```
## commands valid
```
ipconfig getifaddr en0
ng serve -o --host 192.168.1.9
ionic cap run android --external --livereload-url=http://192.168.1.9:4200
```

If you are referring your localhost on your system from the Android emulator then you have to use http://10.0.2.2:8080/ Because Android emulator runs in a Virtual Machine therefore here 127.0.0.1 or localhost will be emulator's own loopback address.
https://stackoverflow.com/questions/5495534/java-net-connectexception-localhost-127-0-0-18080-connection-refused
