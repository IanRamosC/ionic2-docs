Badge
===========

```
$ cordova plugin add cordova-plugin-badge
```

Repositório: [https://github.com/katzer/cordova-plugin-badge](https://github.com/katzer/cordova-plugin-badge)

O principal objetivo dos badges é permitir que um aplicativo informe ao usuário que existe alguma coisa nova — como mensagens não lidas — quando ele não estiver no aplicativo.


Esse plugin tem como dependência: ```cordova-plugin-badge```. Para mais informações, por favor veja a [documentação do plugin Badge](https://github.com/katzer/cordova-plugin-badge).

Platafomas suportadas
-----
- Android
- iOS
- Navegador
- Windows
- Amazon FireOS
- Windows Phone 8

Uso
---

``` javascript
import {Badge} from 'ionic-native';

Badge.set(10);
Badge.increase();
Badge.clear();
```

Métodos estáticos
-----------------

``` clear() ```

Remove o badge do ícone do aplicativo.


``` set(number) ```

Configura o número do badge igual ao valor passado como argumento.

| Parametro                     | Tipo         | Detalhes                                     |
|-------------------------------|--------------|----------------------------------------------|
| number                        | ```number``` | O novo número do badge                  		  |

*Retorna:* ```Promise``` 


``` get() ```

Obtém o número do badge.

*Retorna:* ```Promise``` 


``` increase(count) ```

Adiciona ao número do badge o valor passado como argumento.

| Parametro                     | Tipo         | Detalhes                                     |
|-------------------------------|--------------|----------------------------------------------|
| count                         | ```number``` | Valor para adicionar ao badge atual    		  |

*Retorna:* ```Promise``` 


``` decrease(count) ```

Diminui o número do badge o valor passado como argumento.

| Parametro                     | Tipo         | Detalhes                                     |
|-------------------------------|--------------|----------------------------------------------|
| count                         | ```number``` | Valor para subtrair ao badge atual    	  	  |

*Retorna:* ```Promise``` 


``` hasPermission() ```

Determina se o aplicativo possui permissão para exibir o badge.


``` registerPermission() ```

Registra permissão para configurar o valor do badge.

*Retorna:* ```Promise``` 
