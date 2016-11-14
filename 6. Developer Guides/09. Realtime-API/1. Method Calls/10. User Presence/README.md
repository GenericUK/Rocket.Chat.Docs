# User Presence

Used to set the user presence status. There's two ways to use this call; to set the default status and to set a temporary status.

There're four status available:

- `online`
- `busy`
- `away`
- `offline`

## Setting the default status

In order to set the defult status we need to call the `UserPresence:setDefaultStatus` method passing the status in the parameters of the call.

Example call (setting the user presence to `online`):

```json
{
    "msg": "method",
    "method": "UserPresence:setDefaultStatus",
    "id": "42",
    "params": [ "online" ]
}
```

## Setting a temporary status

Setting a temporary status requires a call to `UserPresence:{status}` with an empty params.

Example call (setting the user presence to `away`):

```json
{
    "msg": "method",
    "method": "UserPresence:away",
    "id": "42",
    "params":[]
}
```