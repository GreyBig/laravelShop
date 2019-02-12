
代码从GitHub拉取下来后需要做的事情：

    composer install
    .env配置数据库
    php artisan key:generate 生成密钥
    使用 Yarn 安装Laravel Mix依赖
    SASS_BINARY_SITE=http://npm.taobao.org/mirrors/node-sass yarn
    webpack.mix.js加上 .version();
    再编译：npm run dev/watch-poll

    本地邮件配置：
    MAIL_DRIVER=smtp
    MAIL_HOST=smtp.gmail.com
    MAIL_PORT=465
    MAIL_USERNAME=greycoder0@gmail.com
    MAIL_PASSWORD=520greycoder
    MAIL_FROM_ADDRESS=greycoder0@gmail.com
    MAIL_FROM_NAME=xiao
    MAIL_ENCRYPTION=ssl

    thinker:
    factory(App\Models\UserAddress::class, 3)->create(['user_id' => 1]) // 创建收货地址数据