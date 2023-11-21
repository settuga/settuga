- 👋 Hi, I’m @settuga
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
settuga/settuga is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
Title: `Could not check out a connection in 5.0 seconds (DB::PoolTimeout)`
Date: `2023-11-21T11:18:55Z`
Route: `/feed/trending`
Version: `2023.11.08-c5b87e3b @ master`

<details>
<summary>Backtrace</summary>
<p>
   
```
Could not check out a connection in 5.0 seconds (DB::PoolTimeout)
  from lib/db/src/db/pool.cr:235:7 in 'wait_for_available'
  from lib/db/src/db/pool.cr:85:35 in 'checkout'
  from src/invidious/yt_backend/connection_pool.cr:33:7 in '_post_json'
  from src/invidious/yt_backend/youtube_api.cr:388:12 in 'browse:params:client_config'
  from src/invidious/trending.cr:19:3 in 'fetch_trending'
  from src/invidious/routes/feeds.cr:55:24 in 'trending'
  from src/invidious/routing.cr:100:27 in '->'
  from lib/kemal/src/kemal/route.cr:12:26 in '->'
  from src/invidious/helpers/handlers.cr:30:5 in 'process_request'
  from lib/kemal/src/kemal/route_handler.cr:17:7 in 'call'
  from /usr/share/crystal/src/http/server/handler.cr:30:7 in 'call_next'
  from lib/kemal/src/kemal/websocket_handler.cr:13:14 in 'call'
  from /usr/share/crystal/src/http/server/handler.cr:30:7 in 'call_next'
  from lib/kemal/src/kemal/filter_handler.cr:21:7 in 'call'
  from /usr/share/crystal/src/http/server/handler.cr:30:7 in 'call_next'
  from src/invidious/helpers/handlers.cr:212:5 in 'call'
  from /usr/share/crystal/src/http/server/handler.cr:30:7 in 'call_next'
  from src/invidious/helpers/handlers.cr:94:12 in 'call'
  from /usr/share/crystal/src/http/server/handler.cr:30:7 in 'call_next'
  from src/invidious/helpers/handlers.cr:145:12 in 'call'
  from /usr/share/crystal/src/http/server/handler.cr:30:7 in 'call_next'
  from src/invidious/helpers/handlers.cr:70:5 in 'call'
  from /usr/share/crystal/src/http/server/handler.cr:30:7 in 'call_next'
  from src/ext/kemal_static_file_handler.cr:162:16 in 'call'
  from /usr/share/crystal/src/http/server/handler.cr:30:7 in 'call_next'
  from lib/kemal/src/kemal/exception_handler.cr:8:7 in 'call'
  from /usr/share/crystal/src/http/server/handler.cr:30:7 in 'call_next'
  from src/invidious/helpers/logger.cr:17:35 in 'call'
  from /usr/share/crystal/src/http/server/handler.cr:30:7 in 'call_next'
  from lib/kemal/src/kemal/init_handler.cr:12:7 in 'call'
  from /usr/share/crystal/src/http/server/request_processor.cr:51:11 in 'process'
  from /usr/share/crystal/src/http/server.cr:521:5 in 'handle_client'
  from /usr/share/crystal/src/http/server.cr:451:5 in '->'
  from /usr/share/crystal/src/fiber.cr:146:11 in 'run'
  from /usr/share/crystal/src/fiber.cr:98:34 in '->'
  from ???
```
</p>
</details>
