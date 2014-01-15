processes
=========

Procfile to get processes running 

Take this Procfile and place it in the root path of the meta-project.  For example, your directories could look like:

```
FooFoBerry
|\
| Procfile
| costner_goes_postal/
| feed_engine_api/
| feed_engine_auth/
| feed_engine_front_end/
| feed_engine_proxy/
```

Then run `foreman start` and all the processes will launch

If you get an error about a port being taken already, run `lsof -i tcp:<port that is taken>` and then go kill that process (`kill -9 <process_id>`).
