# remix-vite css bug

Steps to reproduce

```
- yarn dev
```

```sh
🖲 remix-vite started at http://localhost:3000
1:34:22 AM [vite] Internal server error: URI malformed
      at decodeURI (<anonymous>)
      at viteTransformMiddleware (file:///Users/xpto/.npm/_npx/3a15c32a5195f478/node_modules/vite/dist/node/chunks/dep-c842e491.js:61159:19)
      at call (file:///Users/xpto/.npm/_npx/3a15c32a5195f478/node_modules/vite/dist/node/chunks/dep-c842e491.js:49213:7)
      at next (file:///Users/xpto/.npm/_npx/3a15c32a5195f478/node_modules/vite/dist/node/chunks/dep-c842e491.js:49157:5)
      at file:///Users/xpto/.npm/_npx/3a15c32a5195f478/node_modules/vite/dist/node/chunks/dep-c842e491.js:37473:28
      at viteServePublicMiddleware (file:///Users/xpto/.npm/_npx/3a15c32a5195f478/node_modules/vite/dist/node/chunks/dep-c842e491.js:37519:9)
      at call (file:///Users/xpto/.npm/_npx/3a15c32a5195f478/node_modules/vite/dist/node/chunks/dep-c842e491.js:49213:7)
      at next (file:///Users/xpto/.npm/_npx/3a15c32a5195f478/node_modules/vite/dist/node/chunks/dep-c842e491.js:49157:5)
      at next (file:///Users/xpto/.npm/_npx/3a15c32a5195f478/node_modules/vite/dist/node/chunks/dep-c842e491.js:49135:14)
      at cors (file:///Users/xpto/.npm/_npx/3a15c32a5195f478/node_modules/vite/dist/node/chunks/dep-c842e491.js:49681:7)
      at file:///Users/xpto/.npm/_npx/3a15c32a5195f478/node_modules/vite/dist/node/chunks/dep-c842e491.js:49717:17
      at originCallback (file:///Users/xpto/.npm/_npx/3a15c32a5195f478/node_modules/vite/dist/node/chunks/dep-c842e491.js:49707:15)
      at file:///Users/xpto/.npm/_npx/3a15c32a5195f478/node_modules/vite/dist/node/chunks/dep-c842e491.js:49712:13
      at optionsCallback (file:///Users/xpto/.npm/_npx/3a15c32a5195f478/node_modules/vite/dist/node/chunks/dep-c842e491.js:49692:9)
      at corsMiddleware (file:///Users/xpto/.npm/_npx/3a15c32a5195f478/node_modules/vite/dist/node/chunks/dep-c842e491.js:49697:7)
      at call (file:///Users/xpto/.npm/_npx/3a15c32a5195f478/node_modules/vite/dist/node/chunks/dep-c842e491.js:49213:7)
      at next (file:///Users/xpto/.npm/_npx/3a15c32a5195f478/node_modules/vite/dist/node/chunks/dep-c842e491.js:49157:5)
      at Function.handle (file:///Users/xpto/.npm/_npx/3a15c32a5195f478/node_modules/vite/dist/node/chunks/dep-c842e491.js:49160:3)
      at app (file:///Users/xpto/.npm/_npx/3a15c32a5195f478/node_modules/vite/dist/node/chunks/dep-c842e491.js:49025:37)
      at Layer.handle [as handle_request] (/Users/xpto/.npm/_npx/3a15c32a5195f478/node_modules/express/lib/router/layer.js:95:5)
      at trim_prefix (/Users/xpto/.npm/_npx/3a15c32a5195f478/node_modules/express/lib/router/index.js:328:13)
      at /Users/xpto/.npm/_npx/3a15c32a5195f478/node_modules/express/lib/router/index.js:286:9
      at Function.process_params (/Users/xpto/.npm/_npx/3a15c32a5195f478/node_modules/express/lib/router/index.js:346:12)
      at next (/Users/xpto/.npm/_npx/3a15c32a5195f478/node_modules/express/lib/router/index.js:280:10)
      at SendStream.error (/Users/xpto/.npm/_npx/3a15c32a5195f478/node_modules/serve-static/index.js:121:7)
      at SendStream.emit (node:events:513:28)
      at SendStream.error (/Users/xpto/.npm/_npx/3a15c32a5195f478/node_modules/send/index.js:270:17)
      at SendStream.pipe (/Users/xpto/.npm/_npx/3a15c32a5195f478/node_modules/send/index.js:516:10)
      at serveStatic (/Users/xpto/.npm/_npx/3a15c32a5195f478/node_modules/serve-static/index.js:125:12)
      at Layer.handle [as handle_request] (/Users/xpto/.npm/_npx/3a15c32a5195f478/node_modules/express/lib/router/layer.js:95:5)
      at trim_prefix (/Users/xpto/.npm/_npx/3a15c32a5195f478/node_modules/express/lib/router/index.js:328:13)
      at /Users/xpto/.npm/_npx/3a15c32a5195f478/node_modules/express/lib/router/index.js:286:9
      at Function.process_params (/Users/xpto/.npm/_npx/3a15c32a5195f478/node_modules/express/lib/router/index.js:346:12)
      at next (/Users/xpto/.npm/_npx/3a15c32a5195f478/node_modules/express/lib/router/index.js:280:10)
      at expressInit (/Users/xpto/.npm/_npx/3a15c32a5195f478/node_modules/express/lib/middleware/init.js:40:5)
      at Layer.handle [as handle_request] (/Users/xpto/.npm/_npx/3a15c32a5195f478/node_modules/express/lib/router/layer.js:95:5)
      at trim_prefix (/Users/xpto/.npm/_npx/3a15c32a5195f478/node_modules/express/lib/router/index.js:328:13)
      at /Users/xpto/.npm/_npx/3a15c32a5195f478/node_modules/express/lib/router/index.js:286:9
      at Function.process_params (/Users/xpto/.npm/_npx/3a15c32a5195f478/node_modules/express/lib/router/index.js:346:12)
      at next (/Users/xpto/.npm/_npx/3a15c32a5195f478/node_modules/express/lib/router/index.js:280:10)
      at query (/Users/xpto/.npm/_npx/3a15c32a5195f478/node_modules/express/lib/middleware/query.js:45:5)
      at Layer.handle [as handle_request] (/Users/xpto/.npm/_npx/3a15c32a5195f478/node_modules/express/lib/router/layer.js:95:5)
      at trim_prefix (/Users/xpto/.npm/_npx/3a15c32a5195f478/node_modules/express/lib/router/index.js:328:13)
      at /Users/xpto/.npm/_npx/3a15c32a5195f478/node_modules/express/lib/router/index.js:286:9
      at Function.process_params (/Users/xpto/.npm/_npx/3a15c32a5195f478/node_modules/express/lib/router/index.js:346:12)
      at next (/Users/xpto/.npm/_npx/3a15c32a5195f478/node_modules/express/lib/router/index.js:280:10)
      at Function.handle (/Users/xpto/.npm/_npx/3a15c32a5195f478/node_modules/express/lib/router/index.js:175:3)
      at Function.handle (/Users/xpto/.npm/_npx/3a15c32a5195f478/node_modules/express/lib/application.js:181:10)
      at Server.app (/Users/xpto/.npm/_npx/3a15c32a5195f478/node_modules/express/lib/express.js:39:9)
      at Server.emit (node:events:513:28)
URIError: Failed to decode param '/html,body,div,span,applet,object,iframe,h1,h2,h3,h4,h5,h6,p,blockquote,pre,a,abbr,acronym,address,big,cite,code,del,dfn,em,img,ins,kbd,q,s,samp,small,strike,strong,sub,sup,tt,var,b,u,i,center,dl,dt,dd,ol,ul,li,fieldset,form,label,legend,table,caption,tbody,tfoot,thead,tr,th,td,article,aside,canvas,details,embed,figure,figcaption,footer,header,hgroup,menu,nav,output,ruby,section,summary,time,mark,audio,video%20%7B%20%20margin:%200;%20%20padding:%200;%20%20border:%200;%20%20font-size:%20100%;%20%20font:%20inherit;%20%20vertical-align:%20baseline;%7Darticle,aside,details,figcaption,figure,footer,header,hgroup,menu,nav,section%20%7B%20%20display:%20block;%7Dbody%20%7B%20%20line-height:%201;%7Dol,ul%20%7B%20%20list-style:%20none;%7Dblockquote,q%20%7B%20%20quotes:%20none;%7Dblockquote:before,blockquote:after,q:before,q:after%20%7B%20%20content:%20'';%20%20content:%20none;%7Dtable%20%7B%20%20border-collapse:%20collapse;%20%20border-spacing:%200;%7D'
```
