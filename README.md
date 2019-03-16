# jQuery_review
jQuery practice demo

node 配置jQuery

1.github 新建项目
2.vscode 打开项目并初始化
    npm init -y
3.安装jQuery
    npm install jquery --save-dev
    3.1 新建.gitignore文件
        node_modules/
4.安装jsdom
     npm install jsdom --save-dev
5.新建主入口文件index.js
    官料：
    <!-- require("jsdom").env("", function(err, window) {
        if (err) {
            console.error(err);
            return;
        }
    
        var $ = require("jquery")(window);
    }); -->
    网料：
    const jsdom = require("jsdom");
    const { JSDOM } = jsdom;
    const { window } = new JSDOM(`<!DOCTYPE html>`);
    const $=require('jQuery')(window);
