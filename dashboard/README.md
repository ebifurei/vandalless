# Vandalless
Source code for Vandalless

## System Requirements


## How to Install
1. Clone this repo to your machine
2. Run `composer install`
3. Make `.env` from `.env.example`
4. Fill database section in `.env`
6. run `php artisan key:generate`
7. run `php artisan migrate --seed`
8. run `php artisan storage:link`
10. run `npm install`

## Queue Configuration
### local environment


## Broadcasting Configuration
### Via Pusher
- Create a new Pusher Channel app https://dashboard.pusher.com/
- Fill `PUSHER_APP_ID`, `PUSHER_APP_KEY`, `PUSHER_APP_SECRET`, `PUSHER_APP_CLUSTER`, in `.env` based on your Pusher Channel App Keys
- Change `BROADCAST_DRIVER` to `pusher` in `.env`
### Via Redis and Socket.io
- Prepare a Laravel Echo Server (https://github.com/tlaverdure/laravel-echo-server)
- Change `BROADCAST_DRIVER` to `redis` in `.env`
- Fill `REDIS_BROADCAST_HOST` `REDIS_BROADCAST_PASSWORD` `REDIS_BROADCAST_PORT` `REDIS_BROADCAST_DB` in `.env` according to your Laraver Echo Server Configuration

## Credits
### Main Contributors
- [Aldiansyah Triewicaksono](https://github.com/ebifurei)
### Development

