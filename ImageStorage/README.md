image storage for phoneGap

```javascript
    document.addEventListener('deviceready', function(){

        var url = 'https://secure.gravatar.com/avatar/bb6eeca6c19f5f11c8aaaa061ccde5e7?s=140&d=https://a248.e.akamai.net/assets.github.com%2Fimages%2Fgravatars%2Fgravatar-user-420.png';

        var fileStorage = new ImageStorage({
            root: '/sdcard/TEST/'
        });

        fileStorage.get(url, function(src){
            console.log('get file success: ' + src);
        }, function(){

        });

    }, false);
```