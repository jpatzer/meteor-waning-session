# Waning Session

Logs out a user a specified period of inactivity. Done all client-side.

It works by tracking any of the following events on the body tag of the document.

* `mousemove`
* `click`
* `keydown`
* `touchstart`

These can be further configured if need be.

You can configure the following options for timeout and

```json
{
  "public": {
    "waningInactivityTimeout": 60,
    "waningActivityEvents": "mousemove click keydown touchstart"
  }
}
```

Requires a bootstrap modal package in order to work. There are quite a few options that can be used.

* https://atmospherejs.com/twbs/bootstrap
* https://atmospherejs.com/peppelg/bootstrap-3-modal

Some inspiration taken from (stale-session)[https://github.com/lindleycb/meteor-stale-session].

_TODO_

* Configure timeout based on roles using (meteor-roles package)[https://github.com/alanning/meteor-roles]