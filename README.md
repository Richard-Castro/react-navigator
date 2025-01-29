Criando React Native - Navigator


https://reactnavigation.org

— Tab Navigator—

npm install @react-navigation/native

npx expo install react-native-screens react-native-safe-area-context

npm install @react-navigation/bottom-tabs


— Drawer Navigator —

npm install @react-navigation/drawer

npx expo install react-native-gesture-handler react-native-reanimated

Expo reanimated

Caso nao tenha o arquivo babel.config.js, criar o arquivo e executar o babel no projeto

Colar em babel.config.js

Instalando babel 

npm install --save-dev @babel/core @babel/runtime @babel/preset-env @babel/preset-react babel-loader

npm install --save-dev metro-react-native-babel-preset

 - plugins: [‘react-native-reanimated/plugins’],

Arquivo completo do Babel Config

module.exports = function(api) {
    api.cache(true);
    return{
        presets: ['babel-preset-expo'],
        plugins: ['react-native-reanimated/plugins'], // No meu projeto deu erro, comentei e nao precisou

    };
  };

Colar na tela de configuração principal… ex App.tsx

  import 'react-native-gesture-handler';

  
 — Stack Navigator —

npm install @react-navigation/native-stack
