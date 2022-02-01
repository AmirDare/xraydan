[![Deploy](https://www.herokucdn.com/deploy/button.png)](https://dashboard.heroku.com/new?template=https://github.com/AmirDare/X1vless)

addEventListener(  
    "fetch",event => {  
        let url=new URL(event.request.url);  
        url.hostname="xx.xxxx.xx";//你的heroku域名    
        let request=new Request(url,event.request);  
        event. respondWith(  
            fetch(request)  
        )  
    }  
)  
