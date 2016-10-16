# Laravel Passport build API
Laravel Passport use Oauth 2 to build API

Follow instruction of Matt Stauffer
https://mattstauffer.co/blog/introducing-laravel-passport 

##Configuration

1. Setup 2 virutal hosts: 
`laravel.passport` mount to `laravel_passport/public`
`laravel.consumer` mount to `laravel_consumer/public`

2. Import database `laravel_passport.sql`
Existing 1 user:
`hoaixuimay@gmail.com` / `123456`

3. Go to `http://laravel.consumer` to authorize
Then it will redirect to laravel.passport for authorize. The autherization require login. After authorizating access token will be print out: `{access_token}`

4. Use one of those API clients: Postman, Restful

Try with link `http://laravel.passport/api/user`

Input headers:

`Content-Type application/json`

`Accept application/json`

`Authorization Bearer {access_token}`

See the result.

