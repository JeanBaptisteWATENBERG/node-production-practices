# node-production-practices

## Logging and monitoring

 - use winston to log everything
   - `TRACE` to reproduce
   - `DEBUG` for logs helping to understand code flow
   - `INFO` for tracking what app does regularly
   - `WARN` for normal errors
   - `FATAL/ERROR` for terrible errors
 - logs response statuses and time
   - https://github.com/bithavoc/express-winston
 - add an id per session
 - monitor blocked event loop https://www.npmjs.com/package/blocked
 - monitor memory usage (should be < 1.5 GB) `process.MemoryUsage().rss`
   
